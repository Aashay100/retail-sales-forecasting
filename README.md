# Retail Sales Analytics & Forecasting (Rossmann)

This project explores daily sales data from Rossmann retail stores and builds a forecasting model to predict future sales.  
The goal was to simulate a real business problem: understanding what factors drive sales (promotions, competition, seasonality, store type) and creating a reliable predictive model that can help retailers plan better.

---

## 🔎 What I Did
- Performed **Exploratory Data Analysis (EDA)** to uncover trends, seasonality, and promo/holiday effects.
- Engineered features such as **lags, rolling averages, competition months open, and calendar features**.
- Built and compared models, with **XGBoost** emerging as the best performer.
- Evaluated performance using **RMSE, MAPE, and R²** on a hold-out period.

---

## 📊 Key Outcomes
- Achieved a forecasting accuracy of **YY% (MAPE)** with XGBoost.  
- Identified **promo campaigns, lag features, and competition distance** as the strongest sales drivers.  
- Produced recruiter-friendly visuals like **feature importance** and **actual vs predicted sales** charts.

---

## 🛠 Tech Stack
Python · pandas · scikit-learn · XGBoost · matplotlib · seaborn · Jupyter

---
## 📂 Repo Layout

<details>
<summary>Click to expand</summary>

```
rossmann-analytics-forecasting/
├── notebooks/
│   └── 01_eda_and_modeling.ipynb
├── artifacts/
│   ├── figures/
│   │   ├── feature_importance_top20.png
│   │   └── actual_vs_pred_test.png
│   ├── model/
│   │   ├── model_xgb.pkl
│   │   └── feature_columns.txt
│   ├── reports/
│   │   └── metrics.json
│   └── data/
│       └── rossmann_processed_sample.csv
├── src/
├── requirements.txt
├── README.md
