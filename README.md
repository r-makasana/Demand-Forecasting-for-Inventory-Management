# 🛒 Demand Forecasting for Inventory Management

## 📌 Overview
This project focuses on predicting weekly product demand to help optimize inventory levels and prevent stockouts or overstocking in retail stores.  
It uses the **Walmart Store Sales Forecasting** dataset from Kaggle and applies **machine learning regression techniques** for time series forecasting.

---

## 🎯 Objective
To forecast weekly sales for multiple Walmart stores using historical sales and external factors such as temperature, fuel price, CPI, and unemployment rate.

---

## 🧠 Machine Learning Formulation
- **Type:** Time Series Forecasting / Regression  
- **Target Variable:** `Weekly_Sales`  
- **Features:** Store ID, Department ID, IsHoliday, Temperature, Fuel Price, CPI, Unemployment, Year, Month, Week, Lag Sales  

---

## 🧰 Tech Stack
- **Language:** Python  
- **Libraries:** Pandas, NumPy, Matplotlib, Seaborn, Scikit-learn, XGBoost, Statsmodels  
- **Environment:** Google Colab  
- **Dataset:** [Walmart Store Sales Forecasting (Kaggle)](https://www.kaggle.com/c/walmart-recruiting-store-sales-forecasting/data)

---

## 📊 Project Workflow

1. **Data Collection**
   - Downloaded dataset using Kaggle API in Google Colab.

2. **Data Cleaning & Merging**
   - Merged training, store, and feature datasets into a single DataFrame.
   - Converted date columns and handled missing values.

3. **Exploratory Data Analysis (EDA)**
   - Visualized sales trends, seasonality, and feature correlations.

4. **Feature Engineering**
   - Extracted time-based features: Year, Month, Week.
   - Created lag-based features: Previous Week Sales, Previous Year Sales.

5. **Model Building**
   - Implemented **XGBoost Regressor** for sales prediction.
   - Trained the model with 80% of the data and tested on 20%.

6. **Evaluation**
   - Used **RMSE (Root Mean Squared Error)** for model performance evaluation.
   - Visualized actual vs. predicted sales.

---

## 📈 Results
- Achieved **RMSE ≈ 1200** on test data (varies by store and department).
- Model successfully captures seasonal and temporal sales patterns.

---

## 📂 Folder Structure
