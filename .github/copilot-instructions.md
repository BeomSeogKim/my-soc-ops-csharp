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

## Repo Notes
- Treat `SocOps/` as source of truth; do not use `.solutions/` for active implementation.
- Deployment publishes docs at site root and Blazor output under `/app` (see `.github/workflows/deploy.yml`).
- Link existing docs instead of duplicating:
  - Commands and overview: `README.md`
  - Workshop workflow: `workshop/GUIDE.md`, `workshop/01-setup.md`
  - Contribution policy: `CONTRIBUTING.md`
  - Styling rules: `.github/instructions/css-utilities.instructions.md`, `.github/instructions/frontend-design.instructions.md`
