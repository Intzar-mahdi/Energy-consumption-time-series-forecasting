# ⚡ Energy Consumption Time Series Forecasting

This project forecasts short-term household energy consumption using historical data. It leverages time-based patterns by engineering temporal features and applying multiple forecasting models: **ARIMA**, **Facebook Prophet**, and **XGBoost**. Visualizations are used to compare model predictions with actual energy usage.

---

## 🎯 Objective

Forecast short-term household energy usage based on historical time-stamped data.  
Key tasks:
- Parse and resample energy data
- Engineer time-related features (hour of day, weekday/weekend)
- Compare ARIMA, Prophet, and XGBoost forecasting models
- Visualize actual vs. predicted consumption

---

## 📁 Dataset

**Household Power Consumption Dataset**  
This dataset contains minute-level measurements of electrical power usage in a household.

- Format: `.txt` or `.csv`
- Fields: Date, Time, Global_active_power, Voltage, Sub_metering_1/2/3
- Source: UCI Machine Learning Repository (or equivalent)

---

## 🔧 Features Extracted

The following time-based features were engineered:
- `hour` → Hour of day
- `day_of_week` → Weekday index (0 = Monday)
- `is_weekend` → Boolean flag for weekend
- `month` → Month of year
- `year` → Year of observation

---

## 📊 Models Implemented

| Model        | Description                                           |
|--------------|-------------------------------------------------------|
| **ARIMA**    | Classical statistical model for stationary series     |
| **Prophet**  | Facebook’s model for trend and seasonality handling   |
| **XGBoost**  | Gradient boosting machine learning model for time series |

---

## 📈 Visualization

For each model, the following were plotted:
- Actual vs Forecasted values
- Residual diagnostics (ARIMA)
- Prophet’s trend and seasonality components
- XGBoost feature importance (optional)

---

## 🛠️ Technologies Used

- **Python**
- **Jupyter Notebook**
- **Pandas**, **NumPy**
- **Matplotlib**, **Seaborn**, **Plotly**
- **Statsmodels (ARIMA)**
- **Facebook Prophet**
- **XGBoost**

---

## 🚀 How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/Intzar-mahdi/Energy-consumption-time-series-forecasting.git
📌 Results
ARIMA: Moderate performance after differencing and stationarity check.

Prophet: Handled seasonality and trend well, ideal for quick forecasts.

XGBoost: Strong performance after time feature engineering, no assumptions about stationarity.>

🧠 Learnings
> Importance of preprocessing time series data (e.g., resampling, handling missing values).

> Feature engineering significantly improves ML model performance.

> Classical models are limited without trend/seasonality handling.



