# What-If Sales Pipeline Analyzer (Tableau Next)

## 📌 Overview
Sales leaders constantly ask: *“What happens to my pipeline if win rates drop, or if we add headcount, or if the market shifts?”*  
Today, this analysis requires static parameters, manual tweaking, and exporting to spreadsheets. It’s slow, siloed, and not collaborative.

This project introduces a **Scenario-Driven Sales Pipeline Analyzer** built on **Tableau Next + Salesforce Platform**.  
It enables live toggling between Baseline, Optimistic, and Downturn scenarios — instantly recalculating KPIs, funnel shape, and booking coverage.  

---

## ❌ The Problem
- Sales forecasting is **rigid** — parameters must be hard-coded.  
- Scenario planning happens offline in Excel or Google Sheets, not inside the analytics layer.  
- Switching between “what-if” cases requires re-running dashboards or manual inputs.  
- Leaders lack a **fast, visual, trustworthy** way to compare different futures.

---

## 🔎 Current State
- Tableau and other BI tools allow parameter-based “what-if” analysis.  
- But parameters are **manual, single-user, and limited**:  
  - Example: change “Win Rate” parameter → only one user sees effect.  
  - Multi-factor scenarios (e.g., market index + discount rate + headcount) become clunky.  
- Agentic Copilots in analytics are **still early** — users cannot yet ask:  
  > “Show me the impact on Q4 bookings if market drops 10% and we cut sales reps by 5.”  

---

## 🚀 Our Solution
- Introduce a **Scenarios Layer** (`scenarios.csv`) that defines multiple business environments in one place.  
- Join this scenarios table with the fact table in Tableau Next → every metric dynamically recomputes.  
- Provide a **Scenario Selector** (Baseline / Optimistic / Downturn) → all KPIs, funnels, and trends update instantly.  
- This mimics how Copilot/Slack could auto-toggle scenarios in production.  
- Result: faster, collaborative, and **agent-ready analytics**.  

**Why it’s better:**  
- No more one-off parameter hacks — we centralize assumptions.  
- Enables storytelling: “If the market turns down, here’s how pipeline coverage shifts.”  
- Future-ready: once Tableau Copilot matures, scenarios can be switched via natural language.  

---

## 🧭 Architecture Overview

![Architecture Diagram](docs/shichi_architecture.png)

---

## 🖼️ App Screenshots

| Home Screen | Log Screen | Flower Screen |
|-------------|---------------|----------------|
| ![Home](assets/Home_screen.png) | ![log](assets/Log_screen.png) | ![flower](assets/Flower_screen.png) |

