<!-- l10n-sync: source-file="README.md" -->
<div align="center">

# 🎲 Soc Ops

**Social Bingo para encontros presenciais — construído com VS Code e GitHub Copilot**

Encontre pessoas que correspondam às perguntas. Consiga 5 em uma fileira e ganhe!

[![.NET 10](https://img.shields.io/badge/.NET-10-512BD4?logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/download/dotnet/10.0)
[![Blazor WebAssembly](https://img.shields.io/badge/Blazor-WebAssembly-7B2FBE?logo=blazor&logoColor=white)](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)
[![GitHub Copilot](https://img.shields.io/badge/GitHub-Copilot-000000?logo=github&logoColor=white)](https://github.com/features/copilot)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

[🎮 **Jogar**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) &nbsp;•&nbsp; [📚 **Guia do Lab**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/) &nbsp;•&nbsp; [🚀 **Iniciar Workshop**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview)

</div>

---

## ✨ O que é o Soc Ops?

O Soc Ops é um **workshop prático** onde você transforma um simples aplicativo de Social Bingo em algo incrível usando o **Modo Agente do VS Code** com **GitHub Copilot**. No caminho, você dominará as habilidades-chave do desenvolvimento AI-first.

| ⏱️ Duração | 🎯 Nível | 🛠️ Stack |
|:-----------:|:--------:|:--------:|
| ~1 hora | Intermediário | C# · .NET 10 · Blazor WebAssembly |

---

## 🧠 O que Você Vai Aprender

| | Habilidade | Descrição |
|---|---|---|
| 🧠 | **Engenharia de Contexto** | Ensine a IA sobre seu codebase com arquivos de instruções, tornando as sugestões do Copilot mais precisas e relevantes |
| 🤖 | **Primitivos Agênticos** | Use agentes em segundo plano, agentes na nuvem e fluxos de trabalho personalizados para escalar seu desenvolvimento |
| 🎨 | **Desenvolvimento Design-First** | Deixe a IA iterar na UI enquanto você guia a visão criativa com agentes de design especializados |
| 🧪 | **Desenvolvimento Guiado por Testes** | Construa funcionalidades confiáveis usando agentes TDD com o fluxo Vermelho → Verde → Refatorar |

---

## 📚 Partes do Workshop

| Parte | Título | Tempo | Descrição |
|:-----:|--------|:-----:|-----------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Visão Geral & Lista Rápida | — | Objetivos, pré-requisitos e o que esperar |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Configuração & Engenharia de Contexto | 15 min | Clone, configure e ensine a IA sobre seu projeto |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Frontend Design-First | 15 min | Redesenhe a UI com temas criativos usando o Modo de Plano |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Quiz Master Personalizado | 10 min | Crie perguntas temáticas com agentes personalizados |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Desenvolvimento Multi-Agent | 20 min | Construa novas funcionalidades com TDD e agentes de design |

> 📝 Os guias do lab também estão disponíveis na pasta [`workshop/pt_BR/`](workshop/pt_BR/) para leitura offline.

---

## ✅ Pré-requisitos

Antes de começar, certifique-se de ter:

- [ ] [VS Code](https://code.visualstudio.com/) **v1.107+** (sem atualizações pendentes)
- [ ] Assinatura do **GitHub Copilot** (Pro, Business ou Enterprise) — com sessão iniciada
- [ ] [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) ou superior
- [ ] Git instalado

> 💡 **Dica:** Use o DevContainer para um ambiente pré-configurado com tudo já instalado!

---

## 🚀 Início Rápido

### Opção A — GitHub Codespaces *(recomendado)*

Após criar seu próprio repositório a partir deste template:

1. Abra seu repositório no GitHub
2. Clique em **Code** → **Codespaces** → **Create codespace on main**
3. Aguarde o devcontainer terminar a configuração
4. Execute o aplicativo:
   ```bash
   cd SocOps && dotnet run
   ```

### Opção B — Local

```bash
# Clone o repositório, depois:
cd SocOps
dotnet run        # iniciar servidor de desenvolvimento
dotnet build      # apenas compilar
```

O aplicativo estará disponível em `http://localhost:5166`.

---

## 🌍 Deploy

Pushes para `main` são implantados automaticamente no **GitHub Pages** via GitHub Actions.

---

## 💡 Dicas Pro

1. **Mantenha o navegador aberto** — veja as atualizações ao vivo enquanto codifica
2. **Faça commits com frequência** — salve estados funcionais regularmente
3. **Use checkpoints** — reverta mudanças inesperadas com Checkpoints & Undo do chat do Copilot
4. **Itere nos planos** — refine os planos 2+ vezes antes de implementar

---

<div align="center">

Construído com 💜 pelas equipes do VS Code e .NET

</div>
