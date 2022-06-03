# Time_Series_Analysis

## This Time Series Analysis Of Gold & Silver Repository contains,

##### Gold & Silver Price Prediction using Python(ARIMA).ipynb: Using Autoregressive integrated moving average predicting prices of gold and silver through Yfinance.

An autoregressive integrated moving average, or ARIMA, is a statistical analysis model that uses time series data to either better understand the data set or to predict future trends. 
A statistical model is autoregressive if it predicts future values based on past values. For example, an ARIMA model might seek to predict a stock's future prices based on its past performance or forecast a company's earnings based on past periods.

An autoregressive integrated moving average model is a form of regression analysis that gauges the strength of one dependent variable relative to other changing variables. The model's goal is to predict future securities or financial market moves by examining the differences between values in the series instead of through actual values.

An ARIMA model can be understood by outlining each of its components as follows:
1. Autoregression (AR): refers to a model that shows a changing variable that regresses on its own lagged, or prior, values.
2. Integrated (I): represents the differencing of raw observations to allow for the time series to become stationary (i.e., data values are replaced by the difference between the data values and the previous values).
3. Moving average (MA):  incorporates the dependency between an observation and a residual error from a moving average model applied to lagged observations.

Each component in ARIMA functions as a parameter with a standard notation. For ARIMA models, a standard notation would be ARIMA with p, d, and q, where integer values substitute for the parameters to indicate the type of ARIMA model used. The parameters can be defined as:

p: the number of lag observations in the model; also known as the lag order.
d: the number of times that the raw observations are differenced; also known as the degree of differencing.
q: the size of the moving average window; also known as the order of the moving average.
In a linear regression model, for example, the number and type of terms are included. A 0 value, which can be used as a parameter, would mean that particular component should not be used in the model. This way, the ARIMA model can be constructed to perform the function of an ARMA model, or even simple AR, I, or MA models.

<b>Proceedings:
Building an AutoRegressive Integrated Moving Average (ARIMA) time series machine learning model to forecast the price of Gold & Silver 30 days into the future. Starting off this project by importing all the necessary libraries then downloading real-time data from Yahoo Finance & visualize the historical performance of Gold & Silver through graphs using Matplotlib nextly clearing or segregating out the parameters of ARIMA for modelling purposes finally creating an Arima model and forecast the price 30 days into the future lastly to train, test and evaluate the performance of the model.

Gold Data:
  
  ![image](https://user-images.githubusercontent.com/86974424/171819356-b6871b14-c580-4580-81ef-ea6b1ae5a1bc.png)
  
Data Visualization of Gold:
  
  ![image](https://user-images.githubusercontent.com/86974424/171819416-1c515826-49cd-4949-8276-3cc394b22116.png)

ARIMA Model Parameters:
  
  ![image](https://user-images.githubusercontent.com/86974424/171819589-6cc2e4f9-2d0f-44b2-89fc-25cbfdbaaf93.png)

Model Outcome:
  
  ![image](https://user-images.githubusercontent.com/86974424/171819787-7a3283f4-fdb0-46ca-9d4a-50d4db4f827f.png)
  
Data Visualization of Silver:
  
  ![image](https://user-images.githubusercontent.com/86974424/171819941-d8504d92-2206-4d7e-aaab-531e19f95366.png)

ARIMA Model Parameters:
  
  ![image](https://user-images.githubusercontent.com/86974424/171820014-8bac8ae0-a672-4001-b29c-057f0591a399.png)

Model Outcome:
  
  ![image](https://user-images.githubusercontent.com/86974424/171820101-39bbbacf-d4c3-4307-88f6-2f79967a899d.png)
