<!-- l10n-sync: source-file="README.md" -->
<div align="center">

# 🎲 Soc Ops

**Social Bingo para encuentros presenciales — construido con VS Code y GitHub Copilot**

Encuentra personas que coincidan con las preguntas. ¡Consigue 5 en fila y gana!

[![.NET 10](https://img.shields.io/badge/.NET-10-512BD4?logo=dotnet&logoColor=white)](https://dotnet.microsoft.com/download/dotnet/10.0)
[![Blazor WebAssembly](https://img.shields.io/badge/Blazor-WebAssembly-7B2FBE?logo=blazor&logoColor=white)](https://dotnet.microsoft.com/apps/aspnet/web-apps/blazor)
[![GitHub Copilot](https://img.shields.io/badge/GitHub-Copilot-000000?logo=github&logoColor=white)](https://github.com/features/copilot)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

[🎮 **Jugar**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/) &nbsp;•&nbsp; [📚 **Guía del Lab**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/) &nbsp;•&nbsp; [🚀 **Comenzar Workshop**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview)

</div>

---

## ✨ ¿Qué es Soc Ops?

Soc Ops es un **workshop práctico** donde transformas una simple aplicación de Social Bingo en algo increíble usando el **Modo Agente de VS Code** con **GitHub Copilot**. En el camino dominarás las habilidades clave del desarrollo AI-first.

| ⏱️ Duración | 🎯 Nivel | 🛠️ Stack |
|:-----------:|:--------:|:--------:|
| ~1 hora | Intermedio | C# · .NET 10 · Blazor WebAssembly |

---

## 🧠 Qué Aprenderás

| | Habilidad | Descripción |
|---|---|---|
| 🧠 | **Ingeniería de Contexto** | Enseña a la IA sobre tu codebase con archivos de instrucciones, haciendo las sugerencias de Copilot más precisas y relevantes |
| 🤖 | **Primitivos Agénticos** | Usa agentes en segundo plano, agentes en la nube y flujos de trabajo personalizados para escalar tu desarrollo |
| 🎨 | **Desarrollo Design-First** | Deja que la IA itere en la UI mientras tú guías la visión creativa con agentes de diseño especializados |
| 🧪 | **Desarrollo Guiado por Tests** | Construye funcionalidades confiables usando agentes TDD con el flujo Rojo → Verde → Refactorizar |

---

## 📚 Partes del Workshop

| Parte | Título | Tiempo | Descripción |
|:-----:|--------|:------:|-------------|
| [**00**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=00-overview) | Descripción General & Lista Rápida | — | Objetivos, requisitos previos y qué esperar |
| [**01**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=01-setup) | Configuración & Ingeniería de Contexto | 15 min | Clona, configura y enseña a la IA sobre tu proyecto |
| [**02**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=02-design) | Frontend Design-First | 15 min | Rediseña la UI con temas creativos usando Plan Mode |
| [**03**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=03-quiz-master) | Quiz Master Personalizado | 10 min | Crea preguntas temáticas con agentes personalizados |
| [**04**](https://dotnet-presentations.github.io/vscode-github-copilot-agent-lab/docs/step.html?step=04-multi-agent) | Desarrollo Multi-Agent | 20 min | Construye nuevas funcionalidades con TDD y agentes de diseño |

> 📝 Las guías del lab también están disponibles en la carpeta [`workshop/es/`](workshop/es/) para lectura offline.

---

## ✅ Requisitos Previos

Antes de comenzar, asegúrate de tener:

- [ ] [VS Code](https://code.visualstudio.com/) **v1.107+** (sin actualizaciones pendientes)
- [ ] Suscripción a **GitHub Copilot** (Pro, Business o Enterprise) — con sesión iniciada
- [ ] [.NET 10 SDK](https://dotnet.microsoft.com/download/dotnet/10.0) o superior
- [ ] Git instalado

> 💡 **Consejo:** ¡Usa el DevContainer para un entorno pre-configurado con todo ya instalado!

---

## 🚀 Inicio Rápido

### Opción A — GitHub Codespaces *(recomendado)*

Después de crear tu propio repo desde esta plantilla:

1. Abre tu repo en GitHub
2. Haz clic en **Code** → **Codespaces** → **Create codespace on main**
3. Espera a que el devcontainer termine la configuración
4. Ejecuta la aplicación:
   ```bash
   cd SocOps && dotnet run
   ```

### Opción B — Local

```bash
# Clona el repo, luego:
cd SocOps
dotnet run        # iniciar servidor de desarrollo
dotnet build      # solo compilar
```

La aplicación estará disponible en `http://localhost:5166`.

---

## 🌍 Deploy

Los pushes a `main` se despliegan automáticamente en **GitHub Pages** mediante GitHub Actions.

---

## 💡 Consejos Pro

1. **Mantén el navegador abierto** — observa las actualizaciones en vivo mientras codificas
2. **Haz commits con frecuencia** — guarda estados funcionales regularmente
3. **Usa checkpoints** — revierte cambios inesperados con Checkpoints & Undo del chat de Copilot
4. **Itera en los planes** — refina los planes 2+ veces antes de implementar

---

<div align="center">

Construido con 💜 por los equipos de VS Code y .NET

</div>
