# State-wise-CPI-forecasting
State-wise CPI Forecasting using Time Series. 
## Project Summary
This project applies time series forecasting techniques to predict Consumer Price Index (CPI) inflation trends at the state level. The goal is to model historical CPI data, capture seasonal patterns, and generate accurate short- to medium-term forecasts. By experimenting with ARIMA and SARIMA models, the project demonstrates how seasonality and parameter tuning significantly improve forecasting accuracy for economic time series data.
## Objectives

### 1. Analyze CPI data using decomposition (trend, seasonality, residuals).
### 2. Test for stationarity and apply transformations (Box-Cox, differencing).
### 3. Use ACF/PACF plots to guide model selection.
### 4. Build ARIMA models for forecasting.
### 5. Generate 6-month and 24-month CPI forecasts with confidence intervals.
### 6. Compare observed vs. predicted values to validate model accuracy.

## Results with ARIMA 
The mdoel was able to acheieve RMSE 11 and MAPE 6 because seasonality was not considered and hence future predictiond dont show fluctuations, just a linear line
## Results with SARIMA 
Seasonality matters: Accounting for annual cycles drastically reduced errors.
Model simplicity vs complexity: While ARIMA(2,1,9) gave decent results, SARIMA(3,1,2)(0,1,1,12) achieved better performance with fewer parameters.
Although MAPE was higher in this case, the forecasted values were much more accurate when verified with the real data. 
Forecast reliability: The tuned SARIMA model generates forecasts that align closely with actual CPI movements, making it more robust for policy or business use.
