# Oil Price Prediction using LSTM

This repository contains a project aimed at predicting oil prices using a **Long Short-Term Memory (LSTM)** neural network model. LSTM, a type of recurrent neural network (RNN), is well-suited for time series forecasting tasks due to its ability to capture long-term dependencies in sequential data.

## Project Overview

Accurately predicting oil prices is important for market analysts, businesses, and policymakers. This project utilizes historical oil price data to forecast future prices using the LSTM model. It includes all steps from data preprocessing, model building, hyperparameter tuning, and evaluation of results.

### Key Features:
- **Data Preprocessing**: Handling missing values and scaling the data for optimal performance in LSTM models.
- **LSTM Model Architecture**: Building a sequential LSTM model to learn from the time series data.
- **Model Evaluation**: Assessing the model's performance using standard metrics such as **Mean Squared Error (MSE)** and **Mean Absolute Error (MAE)**.
- **Visualization**: Visualizing predicted vs actual values to compare model accuracy.

## Dataset

The dataset used in this project contains historical oil prices with the following key columns:
- `Date`: The date of the recorded oil price.
- `Close`: The closing price of oil on that date.

Ensure the dataset is clean and formatted as a time series before training the model. Missing values are handled, and the data is scaled using **MinMaxScaler** to ensure the values are within a suitable range for the LSTM model.

## Model

The model used in this project is a **Long Short-Term Memory (LSTM)** network, which is an effective neural network for time series data due to its ability to learn long-term dependencies. The architecture involves:
- **Input Layer**: The number of time steps and features (e.g., oil prices).
- **LSTM Layers**: One or more LSTM layers with a defined number of units (neurons).
- **Dense Layer**: A fully connected layer that outputs the predicted value.
  
The model is trained on historical oil price data and is evaluated on a test set.

### Hyperparameter Tuning

Key hyperparameters of the LSTM model include:
- **Number of LSTM units**: Controls the model's capacity to learn patterns from the data.
- **Batch size**: The number of samples processed before the model's weights are updated.
- **Epochs**: The number of times the learning algorithm works through the entire training dataset.
- **Learning rate**: Determines how much to change the model in response to the estimated error at each update.

A grid search or manual tuning process is used to optimize these hyperparameters for the best model performance.

## Requirements

To run this project, the following libraries are required:

```bash
pip install -r requirements.txt
