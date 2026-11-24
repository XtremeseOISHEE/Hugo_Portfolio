---
title: AirSense Dhaka
date: '2026-01-01'
featured: true
tags:
- Machine learning
- Time series
- Python
summary: Next-hour PM2.5 forecasting and historical pollution analysis for Dhaka.
weight: 3
cover_mark: AQ
image:
  alt_text: AirSense Dhaka demonstration dashboard with month and hour controls, pollution
    indicators and a daily pattern chart.
  caption: Actual historical demo interface. Its original UI uses prediction labels;
    this dashboard does not serve live model inference.
---

**Primary developer · Machine Learning course project · 2026**

Independently implemented a pipeline using 52,262 usable hourly observations from 2016–2022, time and lag features, missing-value handling and a chronological train–test split. Compared Linear Regression, Random Forest, MLP and LSTM.

The best reported MLP results on the 2022 test set were R² 0.8239, RMSE 30.22 µg/m³ and MAE 17.92 µg/m³. These results have not been independently reproduced. Dataset licensing, interpolation leakage and a persistence baseline remain checks for further work.

K-means and PCA support pollution-pattern analysis. The Chart.js dashboard displays historical averages; it does not serve live model predictions.

[Repository and methodology](https://github.com/XtremeseOISHEE/Air-Index-Prediction)
