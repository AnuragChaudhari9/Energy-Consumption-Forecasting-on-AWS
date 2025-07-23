# 📊 Energy Forecasting with SARIMA, XGBoost, and AWS QuickSight

This project forecasts energy consumption using SARIMA and XGBoost, and visualizes the results on AWS QuickSight. It demonstrates real-world forecasting, model comparison, and BI integration using public datasets and AWS cloud services.

---

## 🗂️ Project Overview

- **Goal:** Predict monthly and daily energy consumption.
- **Models:**  
  - SARIMA → for univariate time series (monthly)  
  - XGBoost → for daily prediction using engineered features
- **Cloud Stack:** AWS S3 + QuickSight + SageMaker
- **Visualizations:** Interactive dashboards with QuickSight

---

## 📌 Key Steps

1. **Data Cleaning** – Filtered out `other_kwh`, added time features.
2. **Feature Engineering** – Added month, day, weekend, holiday.
3. **SARIMA Modeling** – Monthly seasonality modeled using statsmodels.
4. **XGBoost Modeling** – Daily prediction with feature importance.
5. **Model Evaluation** – Compared forecast vs actual with MAPE, plots.
6. **Deployment** – Datasets uploaded to **AWS S3** and visualized in **QuickSight**.

---

## 📈 Visualizations (QuickSight)

<img width="1300" height="880" alt="Screenshot (727)" src="https://github.com/user-attachments/assets/eb3fd52c-8386-4f59-b559-6b700596300a" />


---

## 🛠️ Tech Stack

- 🧠 SARIMA (statsmodels)
- ⚡ XGBoost
- 🐍 Python (Pandas, Seaborn, Sklearn)
- ☁️ AWS (S3, QuickSight, SageMaker)

---

## 🧪 Model Metrics

| Model     | Granularity | MAPE (%) |
|-----------|-------------|-----------|
| SARIMA    | Monthly     | XX.X%     |
| XGBoost   | Daily       | YY.Y%     |

---

## 🔍 Folder Guide

| Folder       | Contents                                |
|--------------|-----------------------------------------|
| `notebooks/` | All modeling & EDA Jupyter notebooks    |
| `data/`      | Cleaned and raw CSVs (or S3 links)       |
| `assets/`    | QuickSight chart screenshots             |

---

## 🚀 Future Work

- Automate daily ingestion + forecast
- Integrate with Lambda or Step Functions for pipelines
- Embed QuickSight dashboards into frontend


