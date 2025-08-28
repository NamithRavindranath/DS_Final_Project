Stock_Market_Prediction

This project applies machine learning and deep learning models to predict next-day stock price movement using technical indicators derived from Tesla (TSLA) stock data (2014–2024).

Project Overview: Dataset from Yahoo Finance (daily OHLCV). Target variable: Next-day direction (Up = 1, Down = 0). Features include MACD, RSI, Bollinger Bands, Momentum, Stochastic Oscillator, and Volume Change. Preprocessing involved scaling, handling imbalance, and chronological train-test split to avoid look-ahead bias.

Models Implemented:

Random Forest (with hyperparameter tuning)

XGBoost (gradient boosting, best overall performer)

LSTM (deep learning for sequential dependencies)

Results:

Baseline: ~50% accuracy (random-walk benchmark)

Random Forest: ~53% accuracy, ROC-AUC ~0.55

XGBoost: ~55% accuracy, ROC-AUC ~0.58

LSTM: ~54% accuracy, ROC-AUC ~0.57

Insights:
SHAP analysis highlighted RSI, MACD, and Momentum as the most influential indicators. All ML models outperformed the baseline, with XGBoost achieving the strongest results.
