# Bed Usage Forecasting with Holt's Winter and AutoSARIMA

This repository contains notebooks and evaluation metrics for forecasting the usage of hospital beds in different wards using **Holt's Winter Exponential Smoothing** and **AutoSARIMA** models. The project aims to provide accurate forecasts for the number of hours beds will be used over the next week, leveraging time series forecasting techniques.

## Repository Contents

- **`Holt's_Winter.ipynb`**:
  - Implements Holt's Winter Exponential Smoothing with additive and multiplicative trends and seasonality.
  - Handles recursive 7-day rolling forecasts with refitting using real observed data.
  - Outputs detailed performance metrics: Mean Absolute Error (MAE) and Mean Squared Error (MSE).
  - Generates interactive visualizations of actual vs forecasted values and error metrics.

- **`Auto_Sarima.ipynb`**:
  - Implements AutoSARIMA for automated seasonal ARIMA model selection.
  - Provides a rolling 7-day forecast, recursively refitting models with updated data.
  - Outputs MAE and MSE metrics for error analysis.

- **Evaluation Metrics CSVs**:
  - **`evaluation_results_all_wards_holts.csv`**: Performance metrics for Holt's Winter models.
  - **`evaluation_results_all_wards_autosarima.csv`**: Performance metrics for AutoSARIMA models.
  - Both CSVs store ward-wise MAE and MSE comparisons for better decision-making.

## Key Features

### Holt's Winter
- Supports four variations:
  - Additive trend and seasonality.
  - Additive trend and seasonality with damping.
  - Multiplicative trend and seasonality.
  - Multiplicative trend and seasonality with damping.
- Generates weekly forecasts with dynamic updates using observed data.

### AutoSARIMA
- Automates the ARIMA model selection process using statistical metrics like AIC and BIC.
- Seasonal component handling for 7-day periodicity.
- Provides robust rolling forecasts with real-time model adaptation.

### Evaluation and Visualization
- **Error Metrics**: Both models output MAE and MSE values for each ward and forecasting model.
- **Interactive Plots**: Displays actual vs forecasted values and comparative error bars for all wards.


