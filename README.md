# Implied-volatility-surface-prediction

## Overview

This project focuses on reconstructing missing implied volatility values from an option chain dataset.

The objective is to estimate hidden implied volatility observations using machine learning and financial feature engineering.

## Features

* Datetime preprocessing
* Wide-to-long data transformation
* Strike extraction
* Option type extraction
* Moneyness calculation
* Baseline interpolation model
* CatBoost regression model

## Machine Learning Pipeline

1. Data Loading
2. Exploratory Data Analysis
3. Datetime Feature Engineering
4. Wide-to-Long Transformation
5. Financial Feature Engineering
6. Baseline Interpolation
7. CatBoost Training
8. Submission Generation

## Feature Engineering

* Underlying Price
* Strike Price
* Option Type
* Hour
* Minute
* Time Index
* Moneyness
* Absolute Moneyness

## Results

| Model                | Public MSE |
| -------------------- | ---------- |
| Linear Interpolation | 0.0010366  |
| CatBoost Regressor   | 0.0004491  |

The CatBoost model improved prediction accuracy by approximately 56.7% over the interpolation baseline.

## Tech Stack

* Python
* Pandas
* NumPy
* CatBoost
* Scikit-learn
* Jupyter Notebook

## Repository Structure

```text
implied-volatility-surface-prediction/
├── IV_Surface_Prediction.ipynb
├── submission_v3.csv
├── README.md
├── requirements.txt
```

## Future Improvements

* Cross-validation based model selection
* Ensemble learning approaches
* Advanced implied volatility surface interpolation techniques
