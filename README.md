# About the project

This Python script is designed to model and forecast the monetary aggregate M3 time series data for three major economies: Europe, USA, and Japan. The script performs several key functions:

1. **Data Collection**: It imports historical M3 data from the Federal Reserve Economic Data (FRED) website. The specific data sources are:
   - **Europe**: [MABMM301EZA189N](https://fred.stlouisfed.org/series/MABMM301EZA189N)
   - **USA**: [MABMM301USA189S](https://fred.stlouisfed.org/series/MABMM301USA189S)
   - **Japan**: [MABMM301JPA189N](https://fred.stlouisfed.org/series/MABMM301JPA189N)

   The data was accessed on 20.08.2023.

2. **Stationarity Testing**: The script applies the Augmented Dickey-Fuller (ADF) test to check for stationarity in the time series data.

3. **Autocorrelation and Partial Autocorrelation Analysis**: It visualizes the autocorrelation (ACF) and partial autocorrelation (PACF) plots to identify the properties of the data and guide the selection of appropriate time series models.

4. **ARIMA Modeling**: The script fits ARIMA (AutoRegressive Integrated Moving Average) models to the data for each region, fine-tuning the parameters to achieve the best fit.

5. **Forecasting**: Using the fitted ARIMA models, it forecasts the future values of the M3 monetary aggregate up to the year 2027, covering a 5 years forecast period (from 2023 to 2027), providing insights into potential trends in money supply.

6. **Visualization**: The script also includes plots that visually represent the historical and forecasted M3 values, helping to illustrate trends and model accuracy.

This script was developed as part of a master's thesis and serves as a personal research project aimed at enhancing skills in Python and time series analysis. The forecasts and results presented here are not official projections but are intended as an exercise in applying advanced analytical techniques.
