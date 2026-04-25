🌐 [Português (BR)](README.pt_BR.md) | [Español](README.es.md)

<div align="center">

# 🎲 Soc Ops

**Social Bingo for in-person mixers — built with VS Code & GitHub Copilot**

Find people who match the questions. Get 5 in a row. Win!

[![.NET 10](https://img.shields.io/badge/.NET-10-512BD4?logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/download/dotnet/10.0)
[![Blazor WebAssembly](https://img.shields.io/badge/Blazor-WebAssembly-7B2FBE?logo=blazor&logoColor=white)](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)
[![GitHub Copilot](https://img.shields.io/badge/GitHub-Copilot-000000?logo=github&logoColor=white)](https://github.com/features/copilot)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

[🎮 **Play the Game**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) &nbsp;•&nbsp; [📚 **Lab Guide**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/) &nbsp;•&nbsp; [🚀 **Start Workshop**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview)

</div>

---

## ✨ What is Soc Ops?

Soc Ops is a **hands-on workshop** where you transform a simple Social Bingo app into something amazing using **VS Code's Agent Mode** with **GitHub Copilot**. Along the way you'll master the key skills of AI-first development.

| ⏱️ Duration | 🎯 Level | 🛠️ Stack |
|:-----------:|:--------:|:--------:|
| ~1 hour | Intermediate | C# · .NET 10 · Blazor WebAssembly |

---

## 🧠 What You'll Learn

| | Skill | Description |
|---|---|---|
| 🧠 | **Context Engineering** | Teach AI about your codebase with instructions files, making Copilot suggestions more accurate and relevant |
| 🤖 | **Agentic Primitives** | Use background agents, cloud agents, and custom workflows to scale your development |
| 🎨 | **Design-First Development** | Let AI iterate on UI while you guide the creative vision with specialized design agents |
| 🧪 | **Test-Driven Development** | Build reliable features using TDD agents with the Red → Green → Refactor workflow |

---

## 📚 Workshop Parts

| Part | Title | Time | Description |
|:----:|-------|:----:|-------------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Overview & Checklist | — | Goals, prerequisites, and what to expect |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Setup & Context Engineering | 15 min | Clone, configure, and teach the AI about your project |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Design-First Frontend | 15 min | Redesign the UI with creative themes using Plan Mode |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Custom Quiz Master | 10 min | Create themed quiz questions with custom agents |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Multi-Agent Development | 20 min | Build new features with TDD and design agents |

> 📝 Lab guides are also available in the [`workshop/`](workshop/) folder for offline reading.

---

## ✅ Prerequisites

Before you begin, make sure you have:

- [ ] [VS Code](https://code.visualstudio.com/) **v1.107+** (no pending updates)
- [ ] **GitHub Copilot** subscription (Pro, Business, or Enterprise) — signed in
- [ ] [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) or higher
- [ ] Git installed

> 💡 **Tip:** Use the DevContainer for a pre-configured environment with everything already set up!

---

## 🚀 Quick Start

### Option A — GitHub Codespaces *(recommended)*

After creating your own repo from this template:

1. Open your repo on GitHub
2. Click **Code** → **Codespaces** → **Create codespace on main**
3. Wait for the devcontainer to finish setup
4. Run the app:
   ```bash
   cd SocOps && dotnet run
   ```

### Option B — Local

```bash
# Clone the repo, then:
cd SocOps
dotnet run        # start dev server
dotnet build      # build only
```

The app will be available at `http://localhost:5166`.

---

## 🌍 Deploy

Pushes to `main` deploy automatically to **GitHub Pages** via GitHub Actions.

---

## 💡 Pro Tips

1. **Keep the browser open** — watch live updates as you code
2. **Commit often** — save working states frequently  
3. **Use checkpoints** — revert unexpected changes with Copilot chat Checkpoints & Undo
4. **Iterate on plans** — refine plans 2+ times before implementing

---

<div align="center">

Built with 💜 by the VS Code & .NET Teams

</div>
