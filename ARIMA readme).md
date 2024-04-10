# ARIMA Model for Demand Forecasting

This README documents a Python script that employs the ARIMA (AutoRegressive Integrated Moving Average) model for forecasting demand, specifically applied to weekly data from a car-sharing service. The aim is to utilise the ARIMA model to identify patterns and predict future demand, offering insights that could be instrumental in strategic planning and operational efficiency.

## Description

The script executes several key steps to process, analyse, and forecast demand:

1. **Data Loading:** The script imports demand data from a CSV file.
2. **Data Preprocessing:** 
   - Converts the 'timestamp' column to datetime format and sets it as the index.
   - Interpolates missing values to maintain data consistency.
   - Resamples the data to calculate weekly average demand.
3. **Data Splitting:** Divides the data into training and testing sets for model validation.
4. **ARIMA Modelling:** 
   - Fits the ARIMA model on the training data.
   - Forecasts future demand over the test set duration.
   - Generates confidence intervals for the forecasted values.
5. **Performance Evaluation:** Employs metrics such as mean squared error (MSE), root mean squared error (RMSE), and mean absolute error (MAE) to assess forecast accuracy.
6. **Result Visualisation:** 
   - Plots the historical and forecasted demand along with confidence intervals.
   - Annotates the graph with calculated error metrics.

## Code Overview

The script includes the following key Python libraries: `pandas` for data manipulation, `numpy` for numerical operations, `statsmodels` for the ARIMA model, `matplotlib` for plotting, and `sklearn` for error metrics. It begins by loading the dataset, followed by preprocessing steps like timestamp conversion and missing value interpolation. The script then fits an ARIMA model to the training data, forecasts future demand, and evaluates the forecast's accuracy with error metrics. Lastly, it visualises the training, testing, and forecasted data along with the confidence intervals on a plot.

