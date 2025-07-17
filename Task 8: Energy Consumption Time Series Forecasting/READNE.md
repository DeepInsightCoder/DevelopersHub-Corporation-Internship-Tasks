## Energy Consumption Time Series Forecasting

### Objective

Forecast daily household energy consumption using time series models to anticipate future usage and optimize resource planning.

### Dataset

**Household Power Consumption Dataset**
Columns include:
`Date`, `Time`, `Global_active_power`, `Global_reactive_power`, `Voltage`, `Sub_metering_1`, `Sub_metering_2`, `Sub_metering_3`

### Steps Performed

1. **Data Cleaning & Parsing**

   * Combined `Date` and `Time` into a single `Datetime` column
   * Handled missing values and converted power to numeric

2. **Daily Resampling**

   * Aggregated data to daily level using `.resample('D').mean()`

3. **Modeling**

   * **ARIMA** for statistical forecasting
   * **Facebook Prophet** for additive time series forecasting

4. **Evaluation Metrics**

   * RMSE (Root Mean Squared Error)
   * MAE (Mean Absolute Error)
   * Compared performance of ARIMA vs Prophet

5. **Visualization**

   * Actual vs Forecast plots
   * Residual plots for error analysis

### Results

* Prophet slightly outperformed ARIMA in long-term trend capturing
* NaNs in ARIMA were handled before evaluation
* Visual comparison showed seasonality and forecast confidence intervals

### Skills Gained

* Time Series Forecasting (ARIMA, Prophet)
* Data Resampling & Cleaning
* Forecast Evaluation
* Real-world energy trend analysis
