# NYC Electricity Forecasting – Time Series Modeling with Prophet

This project applies time series forecasting to NYC’s electricity consumption data using Facebook’s Prophet model. It compares multiple forecasting strategies (daily, monthly, yearly) across growth curves to support energy planning and demand analysis.

---

## 🔍 Data Cleaning

- Loaded NYC electricity usage data from 2010–2025.
- Standardized timestamps and removed zero/negative KWH and cost values.
- Aggregated data to **monthly** and **yearly** levels to reduce noise and reveal seasonality.

---

## 📈 Forecasting with Prophet

- Trained Prophet models with **Linear**, **Logistic**, **Flat**, and **Default** growth curves.
- Modeled consumption on daily, monthly, and yearly horizons.
- Evaluated using **MAE**, **MAPE**, and **R²** across forecast windows (1, 10, and 20 years).
- Highlighted seasonal peaks in summer and winter; drops in spring and fall.

---

## 🔬 Model Comparison & Insights

- **Monthly and yearly** models were more stable and predictive than daily due to reduced variance.
- **Linear and logistic growth** yielded the most reliable long-range predictions.
- Daily models struggled with high variability (weather, holidays), common in short-term energy forecasting.
- High **MAPE** values during off-peak periods attributed to small denominator effects.

---

## ✅ Outcomes

- Built a robust, multi-resolution Prophet forecasting pipeline.
- Delivered insights for **grid load management**, **infrastructure planning**, and **sustainability strategy**.
- Enabled scenario testing for future urban energy needs in NYC.

---

## 🛠️ Skills Used

**Tools & Libraries**: Python, Pandas, Prophet, Plotly, NumPy, Matplotlib  
**Techniques**: Time Series Forecasting, Growth Curve Modeling, Data Aggregation, Evaluation (MAE, MAPE, R²)

---

## 📁 Files

- `NYCElectricity.ipynb` – Notebook with EDA and Prophet models  
- `README.md` – This documentation
