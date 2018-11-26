# Web-based-Stock-Forecaster

- Created a Web based Stock Forecaster system with Deep Learning network - Long Short Term Memory (LSTM) and Machine Learning Algorithm - Bayesian Curve fitting for prediction of stock market prices. Efficiency achieved is greater than 95 %.

- Used HTML, CSS, JAVASCRIPT for the front-end.

# Dataset
- Used Aplha Vantage API in python  to to get historical and real-time stock data for each company.
- For each stock, stored the latest day of real-time data and one year of Historical data.
- For each stock, the historical data contains Date, Open, High, Low, Close, Volume data.
- Stored the data in MySQL database.

# Price Indicator
- Used OHLC average (average of Open, High, Low and Closing Prices) for prediction.

# Dataset Preprocessing
- After converting the dataset into OHLC average, it becomes one column data. This has been converted into two column time series data, 1st column consisting stock price of time t, and second column of time t+1. All values have been normalized using MinMaxScaler between 0 and 1.

# Prediction
Long-term Prediction : Used LSTM - Composed of a memory cell, an input gate, an output gate forget gate. It can avoids
the long-term dependencies. It remembers information for periods of time。Two sequential LSTM layers have been stacked together and one dense layer is used to build the RNN model using Keras deep learning library. Since this is a regression task, 'linear' activation has been used in final layer.

Short Term: Used Bayesian Curve Fitting 

# Training
- 75% data is used for training. Adagrad (adaptive gradient algorithm) optimizer is used for faster convergence.

# Result
- The training and testing RMSE are: 1.42 and 1.55 respectively which is pretty good to predict future values of stock.
