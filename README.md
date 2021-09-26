# Time-Series-Modelling
This repository currently contains an attempt to use ARIMA Model to predict future prices on the NASDAQ Composite Index. It contains the following files:

nasdaq_weekly.csv:
- This csv file contains the historical prices for the NASDAQ Composite Index
- The file contains the following columns: Date, Open, High, Low, Close, Adj Close and Volume

Time Series Model - ARIMA:
- This Jupyter notebook contains the code use to read the csv file, fit the data to the ARIMA Model by arriving at the p,d and q terms of the ARIMA Model
- In the second part, the data is split into a training and test set. The test set is the data in more recent times and the aim is to check if the model fitted with the training set is able to predict the future prices as contained in the test set.
- It can be observed towards the end of the notebook that for short look ahead in time, the model is able to predict future prices ie. the prices are within the confidence bands. However, when given a longer time horizon to predict, the predictive accuracy of the model is does not do a good job.
- It is to be noted that the stock market is much too complex to be modelled merely by a univariate time series model. ARIMA model may be more suited a series of data that has more inherent stationarity and also has less factors affecting it.
