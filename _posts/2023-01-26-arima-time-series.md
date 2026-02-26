---
layout: post
title: "ARIMA Time Series Analysis — A Complete Walkthrough"
date: 2023-01-26
description: Step-by-step ARIMA(3,1,0) analysis with 80/20 train-test split, 
             multi-lead forecasting, and diagnostic plots using Python.
tags: [ARIMA, time-series, hydrology, Python, forecasting]
categories: teaching
---

This notebook walks through a complete ARIMA analysis pipeline — from raw 
data to multi-step forecasting — designed for students learning time series 
in hydrology and water resources.

**Topics covered:**
- 80/20 train-test split
- ACF/PACF and stationarity testing (ADF)
- Candidate model comparison (AIC/BIC)
- Full ARIMA(3,1,0) equation derivation (backshift notation)
- One-step-ahead vs recursive multi-step forecasting
- Forecast skill degradation: Lead-1 through Lead-6

## 📓 View the Interactive Notebook

👉 [**Open in nbviewer**](https://nbviewer.org/github/ktripa/DL_Hydrology/blob/main/Class_Execrises_ARIMA_Python.ipynb)

👉 [**View on GitHub**](https://github.com/ktripa/DL_Hydrology/blob/main/Class_Execrises_ARIMA_Python.ipynb)

👉 [**Open in Google Colab**](https://colab.research.google.com/github/ktripa/DL_Hydrology/blob/main/Class_Execrises_ARIMA_Python.ipynb)

---
*The notebook is part of the [DL_Hydrology](https://github.com/ktripa/DL_Hydrology) 
repository. Feedback welcome via GitHub Issues.*

