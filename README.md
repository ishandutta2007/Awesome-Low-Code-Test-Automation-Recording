# Awesome-Low-Code-Test-Automation-Recording

# Awesome Low-Code Test Automation & Recording

> A curated list of top Low-Code Test Automation and Recording platforms — both SaaS/Hosted commercial solutions and open-source alternatives for visually authoring, recording, and maintaining automated tests with minimal coding.
> 🌟 Star this repo if you find it useful! 🌟

---

## 📋 Table of Contents

- [SaaS / Hosted Platforms](#-saas--hosted-platforms)
  - [BrowserStack Low-Code Automation](#browserstack-low-code-automation)
  - [Katalon Studio](#katalon-studio)
  - [mabl](#mabl)
  - [Testim](#testim)
  - [TestRigor](#testrigor)
  - [Leapwork](#leapwork)
  - [Autify](#autify)
  - [AccelQ](#accelq)
- [Open-Source Software](#-open-source-software)
  - [WrightTest](#wrighttest)
  - [INGenious](#ingenious)
  - [HAL-TEST](#hal-test)
  - [TESTAR](#testar)
  - [playwright-recorder](#playwright-recorder)
  - [SessionSnap](#sessionsnap)

---

## 🟦 SaaS / Hosted Platforms

Commercial, cloud-hosted Low-Code Test Automation and Recording platforms. These are not open-source but are included as reference points for feature comparison.

### BrowserStack Low-Code Automation
**Type:** AI-driven recorder with cloud execution and self-healing
BrowserStack's Low-Code Automation provides an intuitive test recorder that captures user actions and transforms them into automated tests without coding . Key capabilities include **AI-powered actions** for natural language automation of complex workflows, **AI-powered validations** for visual accuracy, content, UI elements, and file downloads, **intelligent wait timeouts** to reduce flakiness, **API steps** for setup/teardown, and **custom JavaScript steps** for advanced scenarios . It supports cross-browser testing on desktop and mobile, data-driven testing with CSV files, modules for reusable steps, variables, and secrets management . Tests execute in BrowserStack's cloud without setup, with scheduling, parallel testing, and accessibility testing included .  
**Best for:** Teams wanting a polished, zero-setup recorder with AI-assisted authoring and execution on BrowserStack's device cloud.

### Katalon Studio
**Type:** Low-code IDE with web and mobile recorders
Katalon Studio 11 upgraded its Web and Mobile Recorders with AI-assisted capabilities . The **Web Recording Agent** (Beta) allows describing test scenarios in natural language, which the agent converts into clear test steps and test cases, with a redesigned UI for no-code/low-code users . The **Smart Mobile Recorder** with interactive mode provides a live device preview where taps, swipes, and inputs are automatically turned into test steps . It includes self-healing, Smart Wait, and Time Capsule for debugging . The free tier has limitations; enterprise features require licensing .  
**Best for:** Teams wanting a mature, feature-rich IDE that bridges manual and automated testing with both web and mobile recording.

### mabl
**Type:** Agentic low-code platform with natural language authoring
mabl's agentic testing platform emphasizes creating tests by **describing what you want** in plain English, a user story, or a Jira ticket—no CSS selectors or scripting required . It includes **self-healing** that detects affected tests and handles routine changes automatically, surfacing more significant recoveries for approval . It supports **GenAI Assertions** for validating LLM-generated content, chatbot outputs, and dynamic visuals . mabl claims **up to 85% maintenance reduction** and **90%+ coverage** .  
**Best for:** Teams wanting an AI-native platform where both technical and non-technical members can author and maintain tests through natural language.

### Testim
**Type:** AI-based functional and UI testing with visual editor
Testim is an AI-based functional and end-to-end UI testing solution with a Chrome extension for recording user journeys that are added to a visual editor as discrete, configurable steps . It provides screenshots, console logs, and network info for troubleshooting failed tests, with video capture and annotated screenshots for bug reports . Testim's AI keeps tests stable as code changes .  
**Best for:** Teams wanting a mature visual editor with AI-driven stability and strong debugging artifacts.

### TestRigor
**Type:** AI-driven test automation with plain-language test creation
TestRigor allows creating tests in plain English without coding, with AI that understands intent rather than relying on selectors. It supports web, mobile, and API testing from a single platform.

### Leapwork
**Type:** Visual no-code automation with flowcharts
Leapwork provides a visual, flowchart-based interface for building test automation without coding. It supports web, desktop, and SAP applications, with a focus on enterprise environments requiring cross-application testing.

### Autify
**Type:** AI-powered test automation with visual recorder
Autify provides a visual recorder for creating tests, with AI that maintains tests as applications change. It focuses on web and mobile testing with a no-code approach.

### AccelQ
**Type:** AI-powered codeless test automation
AccelQ provides codeless automation with a visual interface and AI-driven self-healing. It supports web, mobile, API, and desktop testing from a single platform.

---

## 🟩 Open-Source Software

Self-hosted, community-driven Low-Code Test Automation and Recording tools. The open-source ecosystem spans **visual flow builders**, **BDD-based low-code studios**, **node-based automation frameworks**, **scriptless AI testing**, and **focused recording utilities**.

### WrightTest
**Stack:** TypeScript / Playwright / PostgreSQL / Docker | **License:** Open Source (GitHub) 
WrightTest is a low-code UI test automation platform powered by Playwright, with a **no-code recorder**, mobile testing support, and Docker deployment . Key characteristics:
- **Live recording** captures Playwright-ready selectors directly from the browser session, with a noVNC-based interactive view for mobile recording 
- **Data-driven checks** separate the browser flow (Check) from scenario variables (Test Case), allowing one flow to cover multiple scenarios via `{{VARIABLE}}` syntax 
- **Visual editing** of browser checks with global execution history across projects 
- **Mobile testing** via WebKit/Chromium recording and playback 
- **Self-hosted** via Docker Compose with PostgreSQL and Redis 

**Trade-off:** It is a newer project (active as of late 2026) with a focused feature set around browser checks rather than full test management.
**Best for:** Teams wanting a self-hosted, Playwright-powered recorder with data-driven scenarios and mobile support, accepting a newer ecosystem.

### INGenious
**Stack:** (Check repository) | **License:** Open Source (ING)
INGenious is an open-source **Low-Code/No-Code test-automation studio** developed at ING that combines scripted automation with human-readable BDD scenarios . Key characteristics:
- **Reusable steps**: Engineers and business analysts create, maintain, and trace automated tests through reusable steps rather than low-level scripts 
- **BDD-native**: Human-readable scenarios serve as the test definition 
- **AI research integration**: The INGenious–TESTAR collaboration investigated scriptless AI-agents for supportive test scenario generation 

**Best for:** Organizations wanting a BDD-driven low-code studio where business analysts and engineers collaborate on test definition, particularly in enterprise environments.

### HAL-TEST
**Stack:** React / Node.js / Playwright / SQLite | **License:** Open Source (GitHub) 
HAL-TEST is an open-source **visual automation framework for Playwright** that lets developers design and orchestrate browser tests using a **node-based drag-and-drop interface** . Key characteristics:
- **50+ specialized nodes** for DOM manipulation, network interception, and AI 
- **Visual flow editor** with animated execution feedback and real-time test watching 
- **Network orchestration**: Mock, intercept, and modify XHR/Fetch requests visually 
- **Session management**: Persist cookies, local storage, and auth tokens between runs 
- **LLM integration**: Semantic validation and AI-powered node generation 
- **CLI for CI/CD**: Integrated terminal tool for GitHub Actions and Jenkins 
- **Zero vendor lock-in**: Export flows or run via the HAL-TEST CLI 

It uses a monorepo architecture with React Flow, Express, and Playwright, installed via `npx haltest@latest` .
**Best for:** Teams wanting a node-based visual canvas that exposes the full power of Playwright without writing boilerplate, accepting a newer project with a learning curve for the visual paradigm.

### TESTAR
**Stack:** Java | **License:** Open Source (Universitat Politècnica de València) 
TESTAR is a **scriptless, automated, open-source testing tool** developed by the Universitat Politècnica de València and the Open Universiteit of the Netherlands . It is designed for **scriptless AI-driven testing**, automatically exploring applications and generating test scenarios without manual scripting. It was integrated with INGenious for AI-based test scenario generation .  
**Best for:** Teams exploring scriptless, AI-driven exploratory testing without writing test scripts, accepting a research-oriented tool.

### playwright-recorder
**Stack:** Docker / Playwright / X11 | **License:** MIT 
playwright-recorder is a focused **Playwright codegen tool** that runs in Docker with an X11/XWayland display, providing GUI-based recording without polluting your project . Key characteristics:
- **Always fresh**: No reused state, no lockfile pain—ephemeral workspace auto-cleaned 
- **Only generated tests persist**: Output goes to a git-ignored recordings folder 
- **Replay support**: Headless replay of recorded tests without X11 
- **Configurable**: Environment variables for Playwright version, output file, target, and display 

**Trade-off:** It is a **recording utility**, not a full test management or low-code platform—it generates Playwright test code that you then manage yourself.
**Best for:** Developers wanting a clean, isolated Playwright codegen environment without project pollution, accepting that it is a focused tool rather than a platform.

### SessionSnap
**Stack:** CLI / Playwright | **License:** Open Source (GitHub) 
SessionSnap is a CLI tool for **recording and replaying browser sessions** with Playwright, capturing 12 action types (click, dblclick, hover, mousemove, input, select, checkbox, keydown, submit, scroll, file, navigation) . Key characteristics:
- **Interactive or pre-named recording modes**: Start/stop recording with a toolbar, with screenshots and annotations always available 
- **Three-tier selector fallback**: CSS selector → text → coordinates for reliable replay 
- **Noise reduction**: Hover debounced at 150ms, scroll at 400ms, mousemove throttled, keydown only for special keys 
- **Viewport resize protection**: Automatically cancels recording if the window is resized during capture 
- **Named recording management**: Track recordings by name in a profile directory 

**Best for:** Developers wanting a lightweight CLI for capturing and replaying browser interactions with robust selector fallback, accepting a command-line workflow rather than a visual studio.

---

## 📊 Comparison at a Glance

| Software | License | Stack | Visual Recorder | Natural Language | Self-Healing | Self-Hosted | Best For |
|----------|---------|-------|-----------------|------------------|--------------|-------------|----------|
| **BrowserStack** | Proprietary | Cloud | ✅ | ✅ AI actions | ✅ | ❌ | Zero-setup cloud recording |
| **Katalon Studio** | Proprietary | Desktop | ✅ Web + Mobile | ✅ NL to steps | ✅ | ❌ | Mature IDE + mobile recorder |
| **mabl** | Proprietary | Cloud | ✅ | ✅ Intent-based | ✅ GenAI | ❌ | Agentic NL authoring |
| **WrightTest** | Open Source | TS/Playwright/Docker | ✅ Live record | ❌ | (Playwright) | ✅ | Self-hosted Playwright recorder |
| **INGenious** | Open Source | (Check) | (BDD studio) | (BDD steps) | ❌ | ✅ | BDD low-code collaboration |
| **HAL-TEST** | Open Source | React/Node/Playwright | ✅ Node canvas | ✅ LLM nodes | (Designed for) | ✅ | Visual Playwright orchestration |
| **TESTAR** | Open Source | Java | ❌ (Scriptless) | ❌ | (AI-driven) | ✅ | Scriptless exploratory testing |
| **playwright-recorder** | MIT | Docker/Playwright | ✅ Codegen | ❌ | ❌ | ✅ (Docker) | Clean Playwright codegen |
| **SessionSnap** | Open Source | CLI/Playwright | ✅ CLI record | ❌ | (Selector fallback) | ✅ | Lightweight CLI capture/replay |

---

## 🤝 Contributing

Contributions are welcome! If you know of an open-source Low-Code Test Automation or Recording tool that should be listed here, please open a pull request with:

- Project name and URL
- Brief description (1–2 sentences)
- Stack and license
- Why it stands out

Please ensure the project is actively maintained (releases within the last 12 months) and genuinely open-source.

**Note on the open-source ecosystem:** The open-source landscape for **low-code test automation** is **fragmented across distinct approaches** rather than unified platforms. **WrightTest** is the most complete self-hosted option, combining a live Playwright recorder with data-driven scenarios and Docker deployment . **INGenious** offers a BDD-driven studio designed for collaboration between engineers and business analysts . **HAL-TEST** takes a unique node-based canvas approach that exposes Playwright's full power visually . For focused needs, **playwright-recorder** provides clean, isolated codegen in Docker , and **SessionSnap** offers robust CLI-based capture and replay with selector fallback . **TESTAR** represents the scriptless AI-driven end of the spectrum. No open-source project fully replicates BrowserStack's zero-setup cloud execution or mabl's agentic natural language authoring, but these tools cover the core visual recording and low-code authoring workflows for self-hosted deployments.

---

## 📄 License

This list is released under CC0 1.0 Universal (Public Domain). The software projects listed retain their respective licenses.

---

⭐ **If this list helped you discover a useful tool, please star the repo!** ⭐
