# Retail Sales Analytics & Forecasting (Rossmann)

Overview

This project is about predicting how much sales a retail store will make on a given day.
Forecasting sales is critical for retailers because it helps them plan inventory, schedule staff, and design promotions without wasting resources. The aim of this project was to take real sales data and build a model that can forecast future sales more accurately than simple guesswork.

What I Did

I started with historical data that included daily sales, promotions, holidays, and competition details. First, I explored the data to spot patterns — for example, sales are usually higher on weekends, promotions give a noticeable boost, and stores closer to competitors behave differently.

Then I prepared the data for modeling by:

Cleaning missing or inconsistent values

Creating new features like day of week, month, and time since a competitor opened

Encoding store-level information like type and promotions

Finally, I trained and compared different approaches. Simple baselines (like taking the average sales) gave me a starting point, but I then used an XGBoost model, which captured much more of the complexity in the data.

Results

The XGBoost model performed strongly:

RMSE: 952.63 → predictions are on average within ~950 sales of the real numbers

MAPE: 10.05% → forecasts are only about 10% off on average

R²: 0.906 → the model explains about 91% of the variation in sales

This is a big improvement over the baseline models, showing the machine learning approach is much more reliable.

For a business, this means the model could help reduce stock-outs, cut down on overstock, and plan staff shifts more efficiently.

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
