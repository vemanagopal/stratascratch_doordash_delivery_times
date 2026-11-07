# DoorDash Delivery Time Analysis

## Overview

This project explores DoorDash order data and builds regression models to estimate delivery duration. The notebook covers data cleaning, exploratory analysis, feature preparation, model evaluation, and model interpretation.

## Dataset

The analysis uses `historical_data.csv`, which contains order, store, delivery, and dasher-availability information.

- **Raw records**: 197,428
- **Time period**: January–February 2015
- **Target**: Delivery duration in seconds, calculated from order creation to delivery
- Orders placed and delivered on different calendar days are excluded from the analysis.

## Project Structure

```
stratascratch_doordash_delivery_times/
├── doordash_delivery_times.ipynb  # Main analysis
├── historical_data.csv            # Order-level dataset
├── pyproject.toml                 # Python project and dependencies
├── uv.lock
└── README.md
```

## Analysis

The notebook examines feature distributions and correlations, derives calendar features from order time, and compares XGBoost and LightGBM regressors using RMSE and R². It also uses feature importance and SHAP plots to interpret model predictions.
