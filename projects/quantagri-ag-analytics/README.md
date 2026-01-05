# QuantAgri – Agriculture Analytics & Insight Hub

**Live App:** https://quantagri-278412187073.us-west1.run.app

## Overview

QuantAgri is a decision-support platform for agricultural stakeholders, providing data-driven insights into crop yields, pricing trends, and operational risks. The tool combines exploratory analytics with predictive modeling to support both tactical and strategic decisions.

## Problem

Agricultural businesses face uncertainty from weather, market volatility, and supply chain disruptions. Many rely on intuition or outdated spreadsheets rather than data-driven forecasting. QuantAgri bridges this gap with accessible analytics and forecasting tools.

## Data

- **Sources:** (Specify: USDA data, weather APIs, commodity prices, etc.)
- **Granularity:** Daily/weekly/monthly time series
- **Key Variables:**
  - Crop yield metrics
  - Commodity pricing
  - Weather patterns
  - Market indicators

## Approach

### Analytics
- Exploratory data analysis of historical trends
- Correlation analysis between weather, pricing, and yields
- Interactive visualizations for stakeholder exploration

### Predictive Modeling
- **Time Series Forecasting:** Prophet/SARIMA for price and yield predictions
- **Feature Engineering:** Lagged variables, rolling statistics, seasonality indicators
- **Model Evaluation:** Backtesting with MAE/RMSE metrics

## Tech Stack

- **Data Processing:** Python, Pandas, NumPy
- **Modeling:** scikit-learn, Prophet/statsmodels
- **Visualization:** Plotly, Streamlit/Dash
- **Infrastructure:** Docker, GCP Cloud Run

## Key Features

- Interactive dashboards for historical trend analysis
- Forecasting tools for yield and price predictions
- Scenario analysis for risk planning
- Exportable reports for stakeholder communication

## Results

- Provides forward-looking visibility into key agricultural metrics
- Enables data-driven decision making for planting, harvesting, and pricing strategies
- Reduces reliance on heuristic-based planning

