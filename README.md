# Web-based-Stock-Forecaster


- Created a Web based Stock Forecaster system with LSTM network and Bayesian Curve fitting for prediction of stock market prices. Efficiency achieved is greater than 95 %.

- Used HTML, CSS, JAVASCRIPT for the front-end

# Dataset
- Used Aplha Vantage API in python  to to get historical and real-time stock data for each company.
- For each stock, stored the latest day of real-time data and one year of Historical data.
- For each stock, the historical data contains Date, Open, High, Low, Close, Volume data.
- Stored the data in MySQL database.

# Prediction
Long-term Prediction : Used LSTM - Composed of a memory cell, an input gate, an output gate forget gate. It can avoids
the long-term dependencies. It remembers information for periods of time。 

Short Term: Used Bayesian Curve Fitting 

