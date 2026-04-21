# Retail Sales Forecasting

---

## Project Overview

This project focuses on predicting weekly retail sales using historical data from Walmart stores.  
The goal is to build a machine learning model that supports data-driven business decisions such as inventory planning and demand forecasting.

---

## Business Problem

Retail companies need accurate sales forecasts to:

- Optimize inventory levels  
- Reduce overstock and stockouts  
- Improve operational efficiency  

This project simulates a real-world scenario where a company predicts future sales based on historical patterns and external factors.

---

## Dataset

- Source: Walmart Sales Dataset (Kaggle)  
- Includes:
  - Weekly sales data  
  - Store information  
  - External factors (temperature, fuel price, CPI, unemployment, holidays)

---

## Project Workflow

### Data Cleaning
- Merged multiple datasets  
- Converted date fields  
- Handled missing values  

### Exploratory Data Analysis (EDA)
- Identified seasonality patterns  
- Compared holiday vs non-holiday sales  
- Analyzed top-performing stores  
- Observed monthly trends  

### Feature Engineering
- Created time-based features  
- Added lag features  
- Built rolling averages  
- Encoded categorical variables  

### Modeling
- Model: Random Forest Regressor  
- Time-based train/test split  

### Evaluation

| Metric | Value |
|--------|------|
| MAE    | 1,567 |
| RMSE   | 3,341 |
| MAPE   | 15.67% |

---

## Key Insights

- Sales show strong seasonality  
- Lag features significantly improve predictions  
- External factors influence sales  
- A small number of stores drive most revenue  


## Tech Stack

- Python  
- Pandas, NumPy  
- Matplotlib, Seaborn  
- Scikit-learn  
- Jupyter Notebook  

---

## How to Run

1. Clone the repository  
2. Download dataset from Kaggle: https://www.kaggle.com/competitions/walmart-recruiting-store-sales-forecasting/overview 
3. Place files inside `data/` folder  
4. Run
