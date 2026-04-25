# Project Guidelines

## Mandatory Development Checklist
- [ ] Lint: run `dotnet format --verify-no-changes` (or project lint command if configured)
- [ ] Build: run `dotnet build SocOps/SocOps.csproj`
- [ ] Test: run `dotnet test` (when tests exist)

## Architecture
- Single Blazor WebAssembly app (`net10.0`) at `SocOps/SocOps.csproj`.
- Bootstrap/DI: `SocOps/Program.cs`; routing root: `SocOps/App.razor`; main flow: `SocOps/Pages/Home.razor`.
- UI components live in `SocOps/Components`; state orchestration is `SocOps/Services/BingoGameService.cs`; pure bingo logic is `SocOps/Services/BingoLogicService.cs`.
- Models are in `SocOps/Models`; question data is in `SocOps/Data/Questions.cs`.

## Conventions
- Follow standard C# conventions (PascalCase, clear names, nullable-aware code).
- Keep deterministic game rules in `BingoLogicService`; keep persistence/UI transitions in `BingoGameService`.
- Prefer small Razor components with `[Parameter]` and `EventCallback`.
- Reuse utility classes in `SocOps/wwwroot/css/app.css` before adding new styles.

## Design System — Counter-Strike 2 Theme

The app uses a dark tactical aesthetic inspired by CS2's HUD. All design tokens are defined as CSS variables in `SocOps/wwwroot/css/app.css`.

### Color Palette
| Token | Value | Usage |
|---|---|---|
| `--bg-primary` | `#080a09` | Page background |
| `--bg-panel` | `#0f1410` | Card / panel surfaces |
| `--bg-panel-raised` | `#151c15` | Elevated panels |
| `--bg-panel-hover` | `#1c2620` | Interactive hover state |
| `--accent-gold` | `#e8a020` | Primary CTA, winning tiles, headings |
| `--accent-gold-dim` | `#a8700e` | Muted gold, borders |
| `--accent-green` | `#4fa84f` | Marked / confirmed tiles |
| `--accent-green-dim` | `#2a5c2a` | Marked tile borders |
| `--text-primary` | `#d8dcd0` | Body copy |
| `--text-heading` | `#edf0e5` | Headings, prominent text |
| `--text-dim` | `#6b7865` | Hints, labels, secondary text |
| `--border-tactical` | `#2a3328` | Default panel borders |
| `--border-gold` | `#c07a10` | Gold accent borders |

### Typography
- **Headings / UI:** `Rajdhani` (Google Fonts) — bold, uppercase, `letter-spacing: 0.1–0.25em`
- **Monospace / HUD labels:** `Share Tech Mono` (Google Fonts) — terminal/readout text, hints, badges

### Component Class Conventions
- `.bingo-sq` — base square; add `.sq-marked`, `.sq-winning`, `.sq-free` modifiers
- `.hud-panel` — tactical panel with CSS L-corner decorators (no extra markup needed)
- `.start-screen`, `.game-screen` — full-height page wrappers
- `.game-header` — top HUD bar
- `.btn-deploy` — primary CTA button (gold border, fill-on-hover)
- `.btn-abort` — secondary/destructive action (dim text, hover border)
- `.btn-continue` — modal action button (same fill pattern as `.btn-deploy`)
- `.modal-overlay` / `.modal-panel` — victory modal backdrop and card
- `.bingo-banner` — in-game bingo confirmation strip
- `.game-hint` — small monospace instruction bar below header

### Patterns
- **HUD corners:** use the `.hud-panel` class or replicate its `::before`/`::after` pseudo-elements for L-shaped gold corner accents.
- **Grid background:** the `body` already renders a 32px CSS grid pattern; do not add additional background images.
- **Animations:** prefer CSS keyframes already defined in `app.css` (`fade-slide-up`, `glitch-title`, `winning-pulse`, `modal-slide-in`, etc.) before adding new ones.
- **No border-radius on tactical elements:** keep corners sharp (`border-radius: 0`) for HUD panels; only use `rounded-*` utilities for non-tactical UI (e.g., toast notifications).

## Repo Notes
- Treat `SocOps/` as source of truth; do not use `.solutions/` for active implementation.
- Deployment publishes docs at site root and Blazor output under `/app` (see `.github/workflows/deploy.yml`).
- Link existing docs instead of duplicating:
  - Commands and overview: `README.md`
  - Workshop workflow: `workshop/GUIDE.md`, `workshop/01-setup.md`
  - Contribution policy: `CONTRIBUTING.md`
  - Styling rules: `.github/instructions/css-utilities.instructions.md`, `.github/instructions/frontend-design.instructions.md`
