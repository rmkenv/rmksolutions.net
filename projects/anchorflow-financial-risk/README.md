# AnchorFlow – Telemetry & Infrastructure Intelligence Mesh

**Live App:** https://anchorflow-278412187073.us-west1.run.app  

---

## Overview

AnchorFlow is an advanced telemetry and intelligence mesh designed to synthesize fragmented energy infrastructure data into decision-grade insights. It bridges the gap between raw pipeline EBB (Electronic Bulletin Board) filings, maritime transponder signals (AIS), and commodity market indices. By blending real-time monitoring with predictive “What-If” simulations, AnchorFlow enables energy analysts and infrastructure engineers to identify bottlenecks and basis risk before they impact the bottom line.

## Problem

The energy infrastructure sector operates on massive, fragmented datasets. Analysts are often forced to manually correlate pipeline capacity notices, tanker dwell times, and weather-driven demand shifts across multiple siloed platforms. This lagging, incomplete view makes it difficult to quantify regional risk or predict how a single maintenance event might redistribute load across the national grid, leading to reactive decision-making in a high-volatility market.

## Data

- **Sources:**
  - Integrated pipeline telemetry (EBB-style records)
  - Real-time maritime AIS (tanker locations/speeds)
  - Commodity spot price feeds (e.g., Henry Hub)

- **Granularity:**  
  High-frequency gas-day records and live telemetry handshakes.

- **Key Variables:**
  - **Pipeline Throughput:** Scheduled quantities (MMcf) and receipt/delivery signatures  
  - **Infrastructure Health:** 95th-percentile capacity inference and utilization factors  
  - **Maritime Telemetry:** Tanker MMSI, status, speed, and proximity to export terminals  
  - **Market Context:** Henry Hub spot pricing, moving averages (7D/20D SMA), and regional basis risk scores  

## Approach

### Analytics

- **Severity Audit Ranking:** Automated detection of constraint nodes based on peak utilization and high-utilization persistence over time.  
- **Basis Risk Correlation:** Algorithmic scoring that combines localized throughput pressure with market price volatility.  
- **Geospatial Mesh Analysis:** Interactive hub maps using GeoJSON overlays to visualize the physical relationships between pipelines, hubs, and maritime logistics.

### Predictive Modeling

- **7-Day Load Forecasting:** Time-series projections using linear growth models adjusted for seasonality and “weekend factors” via day-of-week decomposition.  
- **What-If Simulation Sandbox:** A maintenance sandbox that allows operators to “disable” nodes and visualize redistribution of load and risk across the secondary mesh.  
- **Grounded AI Reasoning:** Leverages Gemini 3 Pro with Google Search Grounding to verify market claims against live maintenance notices and real-time news, targeting a “zero-hallucination” analytical environment.

## Tech Stack

- **Data Processing:** Custom analytics engine for capacity inference, anomaly detection, and basis-risk scoring  
- **AI Layer:** Google Gemini 3 Pro with Search Grounding for verified intelligence  
- **Frontend:** React 19, Tailwind CSS (industrial UI design)  
- **Visualization:** Recharts (area/line trends), Pigeon Maps (geospatial layers)  
- **Infrastructure:** Dockerized deployment on GCP Cloud Run  

## Key Features

- **Predictive Dashboard:** Overlay of historical throughput with 7-day predictive load profiles.  
- **Interactive Hub Map:** Real-time tracking of infrastructure nodes and LNG tanker clusters.  
- **Maintenance Sandbox:** Tool for simulating operational outages and evaluating secondary bottlenecks in the mesh.  
- **AI Analyst Terminal:** Grounded natural language interface for auditing system telemetry and market news.  
- **Regional Filters:** Ability to slice the national grid by specific production basins (e.g., Permian, Marcellus, Bakken).

## Results

- **Proactive Risk Discovery:** Shifts from reactive monitoring to predictive auditing of infrastructure constraints.  
- **Operational Resilience:** Enables stress-testing of the energy grid under diverse maintenance and outage scenarios.  
- **Verified Intelligence:** Reduces analyst research time by synthesizing maritime, weather, and pipeline data into a single, grounded source of truth.  

---

[← Back to Portfolio](../../README.md)
