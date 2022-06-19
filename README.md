# Time_Series_Analysis

# Gold & Silver Price Prediction using Python(ARIMA): Using Autoregressive integrated moving average predicting prices of gold and silver through Yfinance.

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
##  
Data Visualization of Silver:
  
  ![image](https://user-images.githubusercontent.com/86974424/171819941-d8504d92-2206-4d7e-aaab-531e19f95366.png)

ARIMA Model Parameters:
  
  ![image](https://user-images.githubusercontent.com/86974424/171820014-8bac8ae0-a672-4001-b29c-057f0591a399.png)

Model Outcome:
  
  ![image](https://user-images.githubusercontent.com/86974424/171820101-39bbbacf-d4c3-4307-88f6-2f79967a899d.png)
#  
# Time Series Prediction Platinum: Using Platinum futures time series data from investing.com and predicting/forecasting close price for platinum with 95% confidence bound interval.
  
Dataset: [Platinum Futures](https://www.investing.com/commodities/platinum)
  
Proceedings: 
  
1. Used External API package Investpy to extract historical and recent data with technical indicators of platinum futures dataset in USD. 
  
  ![image](https://user-images.githubusercontent.com/86974424/174474290-205a93c5-49a3-4ef0-b97b-c912b1f35471.png)
  
2. Plotting Closing Price dataset
  
![image](https://user-images.githubusercontent.com/86974424/174474400-7e585437-9200-4b11-be20-8401006bed65.png)

3. Performing ADF test to statisticaly examine the null hypothesis that a unit root exists in an autoregressive time series model. The  alternative hypothesis varies based on the version of the test employed, such as stationarity or trend-stationarity.
  
  ![image](https://user-images.githubusercontent.com/86974424/174474352-3e78d00b-5348-4c20-9b76-4681f2601dfd.png)

4. Obtained rolling mean and standard deviation value for smoothing out data series majorly to identify long—term trends
  
![image](https://user-images.githubusercontent.com/86974424/174474407-6f3b0a50-dd79-48fb-8f6e-85432e061ba6.png)

5. Moving average is calculated to analyze data points by creating a series of averages of different subsets of the full data set of platinum futures it can also be said rolling mean.
  
![image](https://user-images.githubusercontent.com/86974424/174474432-20211d40-d09a-47bb-a0e1-3345758124dc.png)

6. A test stationary function is created to test if the time series properties do not depend on the time at which the series is observed. Thus, time series with trends, or with seasonality, are not stationary — the trend and seasonality will affect the value of the time   series at different times and through our plot it can be said that our series are not stationary.
  
![image](https://user-images.githubusercontent.com/86974424/174474469-80da2e15-5630-4211-bf57-a2cf70806a3e.png)

7. Decomposed my feature to split a time series into several components such as:

~Seasonality: Describing the periodic signal in the time series.
  
~Trend: Describing whether the time series is decreasing, constant, or increasing over time.
  
~Noise: Describing what remains behind the separation of seasonality and trend from the time series. In other words, it’s the variability in the data

![image](https://user-images.githubusercontent.com/86974424/174474529-66aec748-2df6-4298-a245-12e710547922.png)

8. Autocorrelation measures a set of current values against a set of past values to see if they correlate whereas partial Autocorrelation measures the correlation coefficient between a time-series and lagged versions of itself both plots correctly satisfies that our feature is surely correlated with its past and lagged data.

![image](https://user-images.githubusercontent.com/86974424/174474560-022624be-d460-423b-9752-5365df66ef6d.png)

9. Training ARIMA Model:
  
![image](https://user-images.githubusercontent.com/86974424/174474592-9b793f37-14cd-4c87-99e2-27d2299e5aa8.png)

## Model Outcome: At last we can see forecasted plotting with 95% confidence bound interval to see a progressive imbalance in the platinum futures dataset.
Through this plot we can say that for next 10 days close price ranges between 890 to 1100 USD.

![image](https://user-images.githubusercontent.com/86974424/174474628-ac7bc2c8-868a-414e-92c8-82c5a7012cba.png)

### LogScaled Data For Future Platinum Values:
  
![image](https://user-images.githubusercontent.com/86974424/174474663-35fe795b-32f8-40e1-bde7-62df2b983d34.png)






