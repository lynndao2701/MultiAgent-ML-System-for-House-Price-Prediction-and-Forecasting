# 🏠 Multi-agent ML System for House Price Prediction

A hybrid machine learning framework combining supervised learning, time-series forecasting, and metaheuristic optimization to predict and forecast house prices in Australia. The system integrates property-level analysis with market-wide trends using a multi-agent approach.

## 📌 Overview

This project provides accurate house price predictions at both micro (property-level) and macro (state-level) scales. A multi-agent architecture is used:
1. **Micro-level Agent:** Predicts individual property prices using Random Forest, Linear Regression, and Support Vector Regression (SVR).
2. **Macro-level Agent:** Forecasts market trends using ARIMA and LSTM for state-wide housing prices.
⚙️ **Metaheuristic optimization (genetic algorithm)** is used for hyperparameter tuning to improve prediction accuracy.

## ✨ Features
* Hybrid ML system combining regression and time-series models
* Multi-agent architecture for property and market-level analysis
* Hyperparameter optimization using genetic algorithms
* Interactive analysis for understanding key pricing factors
* Robust evaluation using R², RMSE, and MSE metrics

## 📂 Dataset
* **Micro-level Data:** `domain_properties.csv` from Kaggle (11,160 property listings, 17 features)
* **Macro-level Data:** `641606.xlsx` from Australian Bureau of Statistics (ABS) with state-level housing trends
* 🧹 Preprocessing includes handling missing values, encoding categorical features, removing outliers, and generating refined datasets for modeling

## 🛠 Methodology
### Micro-level Agent
* Predicts individual property prices using:
  * Linear Regression (baseline)
  * Random Forest (high accuracy, handles non-linear relationships)
  * Support Vector Regression (robust to outliers, non-linear patterns)
### Macro-level Agent
* Forecasts state-level housing trends using:
  * ARIMA (short-term trends, interpretable)
  * LSTM (captures long-term patterns, seasonal trends)
### Optimization
* Genetic algorithm optimizes ARIMA parameters, LSTM batch size, epoch count, and window size

## ▶️ Usage
1. Preprocess datasets
2. Train micro-level models
3. Train macro-level models
4. Run predictions

## 📊 Results
* Random Forest (micro-level): R² ≈ 0.757, RMSE ≈ 336,505
* Linear Regression: R² ≈ 0.506, RMSE ≈ 479,850
* SVR: R² ≈ 0.367, RMSE ≈ 543,419
* ARIMA (macro-level): Accurate short-term forecasts for 1–2 quarters
* LSTM (macro-level): Captures longer-term trends but limited by dataset size


## 🔮 Future Work
* Integrate additional macroeconomic indicators (e.g., GDP, interest rates)
* Combine ARIMA and LSTM for hybrid short- and long-term forecasting
* Improve model interpretability and user interface
* Explore differential privacy to protect individual transaction data

