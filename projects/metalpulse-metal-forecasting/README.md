# MetalPulse – Smart Metal Forecasting & AI Analytics Hub

**Live App:** https://metalpulse-smart-metal-forecasting-278412187073.us-west1.run.app  

---

## Overview

MetalPulse is a high-fidelity digital nerve center designed for the 2026 commodity super-cycle. It provides institutional-grade insights into precious and industrial metals (Gold, Silver, Platinum, Copper) by blending historical statistical modeling with real-time AI grounding. The platform empowers traders and enthusiasts to visualize “market gravity” while testing their own macro-theses through interactive simulation.

## Problem

In the volatile market landscape of 2026, the **“Sync Gap”**—the delay between global geopolitical shifts and actionable price analysis—has widened. Traditional spreadsheets fail to capture non-linear momentum, and static reports are obsolete by the time they are published. MetalPulse bridges this gap by offering a living, breathing **Pulse** of the market that reacts to live news and user-defined supply/demand biases.

## Data

- **Real-Time Sourcing:** Gemini API with Google Search grounding for live spot price retrieval and market sentiment.  
- **Historical Scope:** Longitudinal price and fundamentals data from 1995 through 2025, providing a 30-year context for multi-degree trend analysis.  
- **Key Variables:**
  - Spot prices (USD/oz and USD/lb)
  - Industrial demand vectors (e.g., photovoltaic growth, EV grid expansion)
  - Monetary indicators (real yields, central bank reserves)
  - Supply constraints (mining stagnation, operational power stability)

## Approach

### Analytics

- **Multi-Model Visualization:** Simultaneous rendering of OLS (linear) and quartic (4th-degree polynomial) regression lines to distinguish between steady growth and high-momentum “blow-off” phases.
- **Driver Decomposition:** Granular breakdown of fundamental drivers (Monetary, Geopolitical, Supply, Demand) with weighted impact scores.
- **Grounding Metadata:** Transparency in AI analysis by extracting and displaying URLs from grounding chunks used in real-time syncs.

### Predictive Modeling

- **Ensemble Forecasting:** Blended approach combining statistical baselines with a 4th-degree polynomial momentum model.
- **Dynamic Sensitivity Logic:** Interactive **Prediction Playground** that applies a time-weighted coefficient to user inputs, simulating how supply/demand shifts ripple through the 2026 forecast horizon.
- **2026 Roadmap:** Quarterly distribution model that weights structural yearly support against seasonal macro headwinds.

## Tech Stack

- **Frontend:** React 19, TypeScript, Tailwind CSS  
- **Intelligence:** Google Gemini API (`@google/genai`) for RAG and search-grounded market updates  
- **Visualization:** Recharts (Area, Line, and Bar composition)  
- **Infrastructure:** ES6 modules via ESM.sh, glassmorphism UI architecture  

## Key Features

- **Live AI Sync:** Instant grounding of 2026 spot prices and market context using the latest Gemini models.
- **Prediction Playground:** Dual-slider interface for **Consumer Craze** and **Metal Scarcity** to adjust ensemble trajectories.
- **2026 Impact Roadmap:** Quarterly **Net Velocity** projections for the current calendar year.
- **Multi-Metal Support:** Specialized datasets and logic for Gold, Silver, Platinum, and Copper.
- **Interactive Methodology:** “Open Methodology” modal detailing the math behind the OLS and quartic models.

## Results

- **Reduced Informational Latency:** Moves the analysis window from “weeks-old reports” to a real-time pulse.
- **Improved Scenario Planning:** Enables “what-if” testing for supply chain disruptions or sudden demand spikes.
- **Democratized Analytics:** Makes complex polynomial regression and fundamental analysis accessible through an intuitive, futuristic interface.

## Architecture

MetalPulse follows a modular, component-driven architecture:

- `App.tsx`: State orchestration and AI service integration.
- `constants.ts`: Structural market data and statistical metadata.
- `HistoricalChart` & `ForecastSection`: Specialized Recharts wrappers for temporal analysis.
- `DriverAnalysis`: Fundamental logic engine for the yearly impact roadmap.

---

[← Back to Portfolio](../../README.md)
