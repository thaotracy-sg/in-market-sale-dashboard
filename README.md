# Electric Power Consumption & CO₂ Emissions Forecasting
## Europe & Central Asia | Time Series Analysis in R

> **Note:** This is an academic project completed as part of the ANL557 Applied 
> Forecasting module at Singapore University of Social Sciences (SUSS), 2025. 
> All data used is publicly available from the World Bank Open Data platform.

## Overview
Applied time series forecasting project analysing electric power consumption 
per capita and its relationship with CO₂ emissions from waste across Europe 
& Central Asia (1981–2023), using World Bank data.

## Key findings
- Electric power consumption shows a clear upward trend: ~21 kWh per capita 
  increase per year (R² = 0.685)
- MA(2) model achieved best overall fit (lowest RMSE, MAE, MAPE)
- Holt's Linear Trend model was most accurate for short-term forecasting 
  (predicted 5,522 vs actual 5,536 kWh in 2023)
- Strong positive correlation (r = 0.829) between electricity consumption 
  and CO₂ emissions — confirming electricity as a reliable emissions proxy
- Forecast: consumption expected to reach ~5,540 kWh per capita by 2024

## Models compared
| Model | RMSE | MAE | MAPE |
|-------|------|-----|------|
| MA(2) | 87.5 | 59.9 | 1.1% |
| Holt's Linear | 88.6 | 60.0 | 1.1% |
| SES | 90.5 | 67.1 | 1.3% |
| ARIMA | 90.5 | 67.2 | 1.3% |

## Tools & techniques
R · tidyverse · ggplot2 · forecast · TTR · ARIMA · Exponential Smoothing · 
Moving Average · ADF Stationarity Test · IQR Outlier Detection · 
Linear Regression Imputation

## Data source
[World Bank — World Development Indicators](https://databank.worldbank.org/source/world-development-indicators)
- Electric power consumption (kWh per capita)
- CO₂ emissions from waste (Mt CO₂e)
- Period: 1981–2023 | Region: Europe & Central Asia
