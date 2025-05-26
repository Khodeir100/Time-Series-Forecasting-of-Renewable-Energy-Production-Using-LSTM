# Time Series Forecasting of Renewable Energy Production Using LSTM

## 📘 Overview

This project focuses on applying time series forecasting techniques to predict renewable energy production in France using Long Short-Term Memory (LSTM) neural networks. The objective is to evaluate model performance for solar and wind energy sources to support more efficient energy planning and management.

The dataset, sourced from [Kaggle](https://www.kaggle.com/), includes hourly production data for intermittent renewable energy sources in France. By transforming the dataset and applying machine learning techniques, this project aims to model and forecast energy outputs with reasonable accuracy.

---

## 🔍 Project Structure


## 📊 Dataset

**Source**: [Kaggle - Intermittent Renewables Production France](https://www.kaggle.com/)

**Fields Used After Preprocessing**:
- `Source` (energy type)
- `Hour`
- `dayOfYear`
- `Year`
- `Production` (energy output)
- `Month`

The data was aggregated from hourly to daily totals for improved forecasting stability.

---

## 🧠 Model & Methodology

- **Model Type**: Long Short-Term Memory (LSTM) Neural Network
- **Input Window**: 28 days of consecutive production data
- **Output**: Forecast for the next day’s energy production
- **Separate Models**: Trained independently for Solar and Wind data

---

## 📈 Results

| Metric | Solar Model | Wind Model |
|--------|-------------|------------|
| MSE    | 2.49        | 2.72       |
| MAE    | 1.21        | 1.27       |
| R²     | 0.34        | 0.52       |

Visualizations comparing actual vs. predicted values are available in the `charts/` directory.

---

## ⚙️ Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/renewable-energy-lstm.git
   cd renewable-energy-lstm
