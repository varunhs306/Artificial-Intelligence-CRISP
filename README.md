# NASDAQ Trend Prediction using CRISP-DM

A machine learning project to predict NASDAQ index trends using the CRISP-DM methodology.

## Overview

- **Objective**: Predict next-day NASDAQ trend (up/down)
- **Data**: 10 years of NASDAQ (^IXIC) data via [yfinance](https://github.com/ranaroussi/yfinance)
- **Models**: Random Forest, XGBoost, LSTM

## Data

| Metric | Value |
|--------|-------|
| Date Range | Dec 2015 - Dec 2025 |
| Total Samples | 2,513 trading days |
| After Cleaning | 2,463 samples |
| Features | 27 (technical indicators, lag features) |

- No missing values in raw OHLCV data
- 50 rows removed after feature engineering (NaN from rolling windows)

## Model Results

| Model | Accuracy | F1 Score |
|-------|----------|----------|
| Random Forest | 42.6% | 0.072 |
| XGBoost | 46.3% | 0.227 |
| **LSTM** | **58.6%** | **0.739** |

## Setup

```bash
pip install -r requirements.txt
```

## Project Structure

```
├── Fin_dashboard.ipynb   # Main analysis notebook
├── requirements.txt      # Dependencies
└── README.md
```

## Authors

- Varun H Shamaraju
- Swaroop K
