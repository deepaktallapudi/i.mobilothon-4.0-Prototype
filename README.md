# i.mobilothon-4.0-Prototype


# AI-Driven Supply Chain Optimization for OEMs

This project focuses on applying various AI and machine learning forecasting methods to predict demand for Original Equipment Manufacturers (OEMs). The goal is to improve supply chain efficiency by accurately forecasting future demand, optimizing inventory, and reducing costs associated with overstocking or stockouts.

## Project Overview

The project leverages different time series forecasting models to predict the future demand based on historical data. Various models were evaluated to determine the best approach for demand forecasting in supply chain management. The models used in this project are:

- **ARIMA (AutoRegressive Integrated Moving Average)**
- **Prophet**
- **LSTM (Long Short-Term Memory)**
- **XGBoost**
- **SARIMA (Seasonal AutoRegressive Integrated Moving Average)**

Each of these models was trained on the historical demand data, and the performance was evaluated using **Mean Absolute Error (MAE)** and **Root Mean Squared Error (RMSE)**.

## Forecasting Models Used

### 1. **ARIMA**
   - **What it is**: ARIMA is a classical time series model that uses historical data to predict future points by considering the dependencies in the data.
   - **Use case**: Ideal for non-seasonal data with trends and autocorrelation.
   - **How it helps in supply chain**: ARIMA helps capture long-term and short-term trends in demand, making it effective for predicting steady, non-seasonal demand fluctuations.

### 2. **Prophet**
   - **What it is**: Prophet is an open-source forecasting tool developed by Facebook, designed to handle missing data and seasonality effectively.
   - **Use case**: Works well with noisy data and missing values, which is common in supply chain forecasting.
   - **How it helps in supply chain**: Prophet accounts for seasonal fluctuations and holidays, making it ideal for forecasting demand that follows specific time-based cycles.

### 3. **LSTM (Long Short-Term Memory)**
   - **What it is**: LSTM is a type of recurrent neural network (RNN) that excels at capturing long-term dependencies in sequential data.
   - **Use case**: Best suited for time series forecasting where past data points have a long-lasting impact on future values.
   - **How it helps in supply chain**: LSTM can identify complex patterns in demand data, taking into account long-term relationships and cyclical trends that influence demand over time.

### 4. **XGBoost**
   - **What it is**: XGBoost is a gradient boosting method that builds an ensemble of decision trees and is known for its speed and accuracy.
   - **Use case**: Highly effective for regression and classification tasks, especially when there are complex, non-linear relationships in the data.
   - **How it helps in supply chain**: XGBoost can model non-linear relationships and interactions between different factors, such as weather, promotions, and seasonal effects, making it ideal for demand forecasting where multiple variables influence the outcome.

### 5. **SARIMA (Seasonal ARIMA)**
   - **What it is**: SARIMA is an extension of ARIMA that accounts for seasonality in the data by incorporating seasonal differencing and seasonal autoregressive terms.
   - **Use case**: Perfect for forecasting data that exhibits repeating cycles, such as product demand with clear seasonal trends.
   - **How it helps in supply chain**: SARIMA can capture seasonal variations in demand, allowing businesses to optimize inventory and production schedules according to expected peaks and troughs in demand.

## Data Collection

For this project, a synthetic dataset was generated to simulate demand data for various products over time. The dataset includes daily demand values and various features such as time of year, holidays, and special events that could affect demand.

## Model Evaluation

The performance of each model was evaluated using the following metrics:
- **Mean Absolute Error (MAE)**: Measures the average magnitude of the forecast errors.
- **Root Mean Squared Error (RMSE)**: Penalizes larger errors and provides an overall measure of how well the model captures trends.

These metrics help determine which model provides the most accurate demand predictions.

## Results and Insights

After applying all the models, we compared their performance using MAE and RMSE. The model with the lowest values for both MAE and RMSE was considered the best performing. This model showed the smallest discrepancies between the predicted and actual demand values, making it the most suitable for use in real-world demand forecasting.

## Conclusion

This project demonstrates how machine learning and AI-driven techniques can be used to optimize supply chain management for OEMs. By accurately forecasting demand using models like ARIMA, Prophet, LSTM, XGBoost, and SARIMA, businesses can improve inventory management, reduce waste, and ensure they meet customer demands efficiently.

## How to Use

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/ai-driven-supply-chain-optimization.git
