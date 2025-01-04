# Coca-Cola and Airline Passenger Data Forecasting

This project demonstrates the process of forecasting Coca-Cola prices and airline passenger data using various time series models. Each model is evaluated based on the RMSE (Root Mean Squared Error) values, and the best model is selected for accurate forecasting.

## Objective
The goal of this project is to apply different time series forecasting models to predict Coca-Cola prices and airline passenger counts. The models are evaluated using RMSE values, and the most suitable model is selected for final predictions.

## Models Used
The following forecasting models were implemented for both the Coca-Cola and Airline Passenger datasets:

1. **Linear Model**  
   A basic approach assuming a linear trend in the data.

2. **Exponential Model**  
   Captures data that grows or decays exponentially over time.

3. **Quadratic Model**  
   A second-order polynomial model, capturing more complex trends.

4. **Additive Model**  
   A simple model where trends, seasonality, and error components are added together.

5. **Additive Seasonality Model**  
   A model that accounts for additive seasonal components.

6. **Multiplicative Model**  
   A model where trends, seasonality, and errors are multiplied together, often suitable for data with exponential growth.

## Data Overview

### Airline Passengers Data
The dataset contains monthly data of airline passengers from 1949 to 1960, capturing seasonal trends and passenger counts. The following models were used to forecast the data:

- **Additive Seasonality Model**: RMSE = 126.278691
- **Additive Seasonality Quadratic Model**: RMSE = 126.278691

### Coca-Cola Price Data
This dataset captures the price data of Coca-Cola over time. The following models were applied:

- **Additive Seasonality Model**: RMSE = 1.460752e-10
- **Additive Seasonality Quadratic Model**: RMSE = 1.460752e-10
- **Quadratic Model**: RMSE = 1857.724
- **Linear Model**: RMSE = 1889.704
- **Multiplicative Seasonality Model**: RMSE = 3321.466
- **Exponential Model**: RMSE = 4392.796

## Dummy Variables Created

For both the Coca-Cola and airline passenger datasets, the following dummy variables were created to handle seasonality and trends:

- **Month Dummy Variables**: Representing each month as a separate variable to capture seasonal effects.
- **Trend Variables**: To model the general upward or downward trend in the data over time.
- **Error Terms**: For capturing residual errors that are not explained by the model.

These dummy variables help in making the models more flexible and capable of capturing complex patterns in the data.

## RMSE Analysis

The following RMSE values were calculated for each model:

### Airline Passenger Data RMSE Values:
- **Additive Seasonality**: 126.278691
- **Additive Seasonality Quadratic**: 126.278691

### Coca-Cola Price Data RMSE Values:
- **Additive Seasonality**: 1.460752e-10
- **Additive Seasonality Quadratic**: 1.460752e-10
- **Quadratic**: 1857.724
- **Linear**: 1889.704
- **Multiplicative Seasonality**: 3321.466
- **Exponential**: 4392.796

## Model Selection

After evaluating the RMSE values for each model, we can conclude the following:

1. For **Airline Passenger Data**, the **Additive Seasonality** and **Additive Seasonality Quadratic** models yield the same RMSE value of 126.278691, making them the best models for forecasting.
   
2. For **Coca-Cola Price Data**, the **Additive Seasonality** and **Additive Seasonality Quadratic** models outperform the other models, with a near-zero RMSE of 1.460752e-10, indicating excellent predictive accuracy.

## Conclusion
The **Additive Seasonality** and **Additive Seasonality Quadratic** models are the best choices for forecasting both Coca-Cola prices and airline passenger data, based on their low RMSE values. These models effectively capture the seasonal components in both datasets and provide reliable forecasts.

## How to Run the Project

1. Clone the repository:
   ```bash
   git clone https://github.com/R-Mahesh45/Forcasting.git
   ```

2. Install necessary dependencies:
   ```bash
   pip install -r requirements.txt
   ```

3. Run the forecasting scripts for Coca-Cola or Airline data in the respective directories.
