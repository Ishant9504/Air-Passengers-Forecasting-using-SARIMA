 ✈️ Air Passengers Forecasting using SARIMA

This project demonstrates how to forecast monthly airline passenger numbers using classical time series modeling techniques — specifically the **Seasonal ARIMA (SARIMA)** model. The dataset spans from **January 1949 to December 1960**, and the model predicts the next **24 months (2 years)** of passenger traffic.

---

## 📊 Project Goals

- Understand and visualize time series components: **trend, seasonality, and noise**
- Test and achieve **stationarity** using the **Augmented Dickey-Fuller (ADF)** test
- Apply **first-order differencing** to stabilize the series
- Use **ACF and PACF plots** to identify optimal ARIMA parameters
- Build and train a **SARIMA** model with both trend and seasonality
- Forecast future values
- Visualize predictions with confidence intervals

---

## 🔧 Tools & Libraries

- `Pandas` for data handling
- `Matplotlib` and `Seaborn` for visualization
- `Statsmodels` for time series modeling

---

## 📁 Key Files

| File                    | Description                                       |
|-------------------------|---------------------------------------------------|
| `air_passengers_forecast.ipynb` | Main Jupyter notebook with full analysis pipeline |
| `forecast.csv`          | Forecasted values with lower and upper confidence intervals |


---

## 📈 Techniques Used

- Seasonal decomposition (trend + seasonality)
- ADF stationarity testing
- ACF and PACF diagnostics for parameter selection
- SARIMA modeling: `(p,d,q)x(P,D,Q,s)`
- Forecast visualization with 95% confidence intervals

---

## 📌 Model Summary

- Chosen Model: `SARIMAX(2, 1, 1)x(1, 0, [1, 2, 3], 12)`
- Model selected based on lowest **AIC**
- Forecast horizon: **24 months** (2 years)

---

## ✅ Forecast Sample

| Date     | Forecast | 95% CI Lower | 95% CI Upper |
|----------|----------|---------------|--------------|
| 1961-01  | 435.2    | 410.6         | 459.8        |
| 1961-02  | 428.7    | 405.3         | 451.4        |
| ...      | ...      | ...           | ...          |

---
