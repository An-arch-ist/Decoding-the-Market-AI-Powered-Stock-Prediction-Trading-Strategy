# Decoding-the-Market-AI-Powered-Stock-Prediction-Trading-Strategy
📈 AI-Powered Stock Forecasting & Portfolio Strategy

This project combines machine learning, econometric forecasting, and portfolio analysis to study stock-market behavior across 10 NSE-listed stocks representing 10 different industries, using approximately 2 years of daily market data. The analysis uses Open, High, Low, Close and Volume data and applies feature engineering, including 3 trading features—Open–Close difference, High–Low range, and 1-day return—with an 80:20 train-test split and approximately 492 observations per stock.

The first component develops a Support Vector Classifier (SVC) to generate next-day Buy/Sell signals, trained on approximately 393 trading days and evaluated on 99 unseen days per stock. The model achieved an average accuracy of approximately 52%, with TCS recording the highest accuracy at 60.6% and Larsen & Toubro the lowest at 41.4%. An equal-weighted SVC portfolio was also evaluated against the NIFTY 50, with the project reporting a portfolio value of 0.0790 versus 0.0006 for NIFTY 50, representing a 0.0784 difference.

The second component focuses on stock-price forecasting using SARIMAX, Support Vector Regression (SVR), XGBoost, and a Hybrid SARIMAX–SVR model. SARIMAX incorporates a 5-day seasonal cycle, while SVR and XGBoost use the previous 3 trading-day prices as lagged predictors. Models were evaluated using MSE, RMSE, MAE and R² across all 10 stocks.

The model comparison found that SVR performed best for 9 of 10 stocks, with an average R² of approximately 0.76, while SARIMAX performed best for Bajaj Finance. The Hybrid SARIMAX–SVR model achieved the strongest overall performance, recording an average MSE of 1,245, RMSE of 26.9, MAE of 19.3 and R² of 0.86, outperforming standalone SVR (R² 0.78), XGBoost (R² 0.38) and SARIMAX (R² −2).

Tools & Techniques: Python, Pandas, Scikit-learn, Statsmodels, XGBoost, Matplotlib, SVC, SARIMAX, SVR, XGBoost, feature engineering, time-series forecasting, model evaluation, portfolio analysis and comparative benchmarking against NIFTY 50.
