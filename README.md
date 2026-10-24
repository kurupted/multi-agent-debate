# AI Council: Multi-Agent Debate & Consensus Engine (v1.0)

> Poses your query to multiple AI models who independently analyze, cross-critique each other's arguments, and produce an evidence-based consensus verdict.

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![Version: 1.0](https://img.shields.io/badge/Version-1.0-emerald.svg)](https://github.com/kurupted/multi-agent-debate)

---

## 🌟 Overview

**AI Council** is a 100% client-side web application designed to counter single-model bias, hallucinations, and blind spots. By orchestrating a structured multi-round debate among diverse frontier and open-weight LLMs via [OpenRouter](https://openrouter.ai), it extracts nuanced, battle-tested answers to complex questions.

### 🏛️ The 3-Round Council Architecture

1. **Round 1 — Blind Independent Analysis:** Council members (e.g., Gemini, Claude, GPT, Nemotron) generate their initial stances in parallel without seeing other models' responses.
2. **Round 2 — Peer Cross-Critique:** All Round 1 perspectives are compiled and fed back to each council member, who cross-examine the arguments, identify flaws or unproven assumptions, and refine their conclusions.
3. **Round 3 — Chief Arbiter Synthesis:** A designated Judge model (e.g., Grok, Claude Opus, Gemini Argon) evaluates all peer critiques, separates facts from speculation, and synthesizes the definitive consensus verdict.
4. **Interactive Follow-Up:** Interrogate the council or converse directly with specific agents or the Judge to probe specific details.

---

## ✨ Features

- **100% Client-Side & Private:** No backend servers, no analytics, and no database. All API calls go directly from your browser to OpenRouter.
- **Model Flexibility:** Choose from pre-configured council lineups (Heavy Reasoning, Speed & Economy, Top Open-Weight, Free $0/M tokens) or plug in any model available on OpenRouter.
- **Automatic Display Names:** Member names and Judge roles automatically adapt as you change models in settings.
- **Domain Presets:**
  - 🚀 **Business Strategy, Ideation & Ventures:** Viability, monetization, automation potential, unit economics, and competitive moats.
  - 📊 **Operations, Workflows & Problem Solving:** Root-cause diagnostics, bottleneck removal, and execution planning.
  - 💻 **Software Architecture & Code Audit:** Scalability, security, trade-offs, and maintainability.
  - 📈 **Investment & Due Diligence:** Valuation, macroeconomic drivers, and risk-reward asymmetry.
  - 🩺 **Medical & Pharmacology:** Evidence hierarchy prioritizing human RCTs over in-vitro theory.
  - ⚖️ **Legal & Regulatory Policy:** Statutory analysis, precedent, and compliance risk.
  - 🧠 **General Truth & Logic:** Objective first-principles reasoning and cognitive bias mitigation.
- **Session Management:** Full debate logs saved to local storage, searchable history drawer, and one-click JSON export/import.
- **API Key Auto-Load:** Automatically reads your OpenRouter key from local files (`.env`, `key.txt`, or `config.json`) when hosted locally.

---

## 🚀 Quick Start

### Running Locally (No installation needed)
Simply open `index.html` (or `multiagent.html`) in any modern web browser:

1. Clone the repository:
   ```bash
   git clone https://github.com/kurupted/multi-agent-debate.git
   cd multi-agent-debate
   ```
2. Double-click `index.html` to open it in your browser.
3. Click **Council & Keys** in the top navigation bar to enter your OpenRouter API key.
   *(Optional: Place a `.env` or `key.txt` file containing your OpenRouter key in the same directory for automatic loading).*
4. Select a **Domain Preset**, type your question, and click **Deliberate & Synthesize**.

---

## 📄 License

This project is licensed under the [GNU General Public License v3.0](LICENSE).
