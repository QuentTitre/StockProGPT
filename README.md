# StockProphetGPT: A Data-driven Approach to Predicting Stock Price

## About The Project 

<p align="justify"> 
  I've alaways had a intrest in stock and options trading. It can be a risky and volatile endeavor. I wanted to find a way the process easier and more profitable with more informed decisions. This project aims to automate the analysis and forecasting of stock prices using machine learning techniques and financial indicators. By leveraging historical stock data and options chain information, the project seeks to provide insights into stock behavior and forecast price movements.
</p>

## Key Componenets
<p align="Justify">
  
1. Data Collection:
Historical stock price data is retrieved using the Yahoo Finance API (yfinance).
Options chain data is obtained for a specified ticker symbol to analyze call and put options.

2. Data Preprocessing: 
Missing values are handled by dropping rows with missing data.
Various financial indicators are calculated, including Simple Moving Average (SMA), Relative Strength Index (RSI), Exponential Moving Average (EMA), Moving Average Convergence Divergence (MACD), Volume Weighted Average Price (VWAP), Bollinger Bands, Stochastic Oscillator, Average True Range (ATR), On-Balance Volume (OBV), Money Flow Index (MFI), and Chaikin Money Flow (CMF).

3. Time Series Analysis:
Augmented Dickey-Fuller (ADF) test is conducted to check for stationarity in the stock price time series data.
LSTM (Long Short-Term Memory) neural network model is trained on the preprocessed data for time series forecasting.

4. Model Training and Evaluation:
The LSTM model is trained using historical stock data with features engineered from financial indicators.
The model is evaluated using mean squared error (MSE), mean absolute error (MAE), and R-squared metrics on a test set.
Predictions are made for future stock prices using the trained model.

6. Visualization:
Historical and predicted stock prices are visualized using matplotlib to provide a clear understanding of model performance and forecasted trends.
</p>

## Conclusion
<p align="Justify">
This project demonstrates an automated pipeline for stock analysis and forecasting, incorporating both technical indicators and machine learning techniques. By utilizing historical data and options chain information, investors can gain valuable insights into stock behavior and make informed decisions regarding trading strategies.
</p>

## Future Work
<p align= "Justify">
1. Adding real time data so the model is continuously learning as market data comes in.
2. Incorporating sentiment analysis from news articles or social media data for additional insights.
3. Implementing ensemble methods or alternative machine learning algorithms for comparison.
4. Building a web interface for easy access and visualization of analysis results.
Overall, the project offers a robust framework for automated stock analysis and forecasting, empowering investors with tools to navigate the dynamic financial markets.
</p>
