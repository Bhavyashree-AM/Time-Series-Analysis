# Time Series Analysis & Forecasting on Seasonal and Non-Seasonal Datasets

## Project Overview

This project applies the Box-Jenkins method to analyze and forecast time series data using ARIMA and GARCH models. The project demonstrates the methodology on two datasets:
- **Capital Bikeshare System**: A non-seasonal dataset containing hourly and daily rental bike counts from 2011-2012, along with weather and seasonal information.
- **Sunset Timings**: A seasonal dataset consisting of monthly average sunset timings from April 2004 to April 2023.

The goal is to showcase the effectiveness of the Box-Jenkins method, ARIMA, and GARCH models for time series analysis, forecasting, and volatility modeling. The project aims to provide insights for decision-making in fields such as bike-sharing systems, agriculture, transportation, and tourism.

## Motivation and Introduction

This project explores how time series analysis can be applied to both seasonal and non-seasonal data, using the Box-Jenkins methodology and various models:
- **Capital Bikeshare Dataset**: Understanding the demand for bike rentals and the impact of external factors.
- **Sunset Timings Dataset**: Analyzing seasonal trends and predicting future sunset times.

## Methodology

The methodology follows the Box-Jenkins steps to analyze and forecast time series data:

### Step 1: Stationary Check
- Perform the **Dicker-Fuller test** to check for stationarity.
- If the data is non-stationary, apply differencing, detrending, or transformation until stationarity is achieved.

### Step 2: Model Selection
- Use **ACF** and **PACF** plots to determine the appropriate model.
- If the plots are unclear, use the **EACF** method for clearer parameter identification.

### Step 3: Parameter Estimation
- Estimate model parameters based on metrics like **AIC**, **BIC**, and **log-likelihood**.
  
### Step 4: Residual Analysis
- Verify model accuracy using **ACF plots**, **QQ plots**, **histograms**, and the **Shapiro-Wilk test**.

### Step 5: Forecasting
- Apply **ARIMA** for non-seasonal data and **SARIMA** for seasonal data.
- Use **GARCH** models for volatility modeling of residuals.
- Evaluate model accuracy using **Mean Absolute Error (MAE)**, **Mean Squared Error (MSE)**, and **Root Mean Squared Error (RMSE)**.

## Data Description

### Capital Bikeshare System (Non-Seasonal Dataset)
- **Data Source**: Hourly and daily bike rental counts between 2011-2012, along with weather and seasonal information.
- **Purpose**: Analyze demand patterns and the impact of external factors on bike-sharing system usage.

### Sunset Timings (Seasonal Dataset)
- **Data Source**: Monthly average sunset timings from April 2004 to April 2023.
- **Purpose**: Analyze seasonal patterns in sunset timings and predict future values.

### Key Features:
- **Genotype**: Control or trisomic (for the Capital Bikeshare dataset).
- **Behavior**: Mice behavior (for behavioral prediction studies).
- **Treatment**: Influence of external factors such as memantine.

## Results

- **Non-Seasonal Forecasting**: Successfully applied the Box-Jenkins method to forecast future bike rental demand.
- **Seasonal Forecasting**: Demonstrated the use of SARIMA and GARCH models to predict sunset timings and model volatility.
  
### Key Findings:
- Achieved accurate forecasts using **ARIMA(1,1,1)** for non-seasonal data.
- Used **SARIMA(2,1,2)x(1,1,0)** for seasonal data with successful results.
- **GARCH(3,1,3)** model effectively captured residual volatility.

## Conclusion

This project demonstrates the successful application of the Box-Jenkins methodology and ARIMA/GARCH models for time series forecasting. The results show the potential of these models in handling both seasonal and non-seasonal datasets, providing accurate forecasts that can aid decision-making in fields such as bike-sharing systems, agriculture, and transportation.

## Future Work

- Extend the analysis to include additional external factors like holidays, weather, etc., in the Capital Bikeshare dataset.
- Apply other advanced models for time series forecasting and volatility modeling.
  
## Technologies Used

- **R**: For statistical analysis and modeling.
- **Time Series Analysis**: ARIMA, SARIMA, GARCH models.
- **Data Visualization**: ACF/PACF plots, residual analysis.

