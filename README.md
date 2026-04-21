# Retail Sales Forecasting

## Project Overview

This project predicts weekly retail sales using historical Walmart store data.
The objective is to build a machine learning model that supports data-driven decisions such as demand forecasting, inventory planning, and operational optimization.

## Business Problem

Retail companies need accurate forecasts to:
- optimize inventory levels
- reduce overstock and stockouts
- improve operational efficiency

This project simulates a real-world forecasting scenario using historical sales data and external economic and seasonal factors.

## Dataset

Source: Walmart Sales Dataset (Kaggle)

The dataset includes:
- weekly sales records
- store-level information
- external variables such as temperature, fuel price, CPI, unemployment, and holiday indicators

## Project Workflow

### Data Cleaning
- merged multiple datasets into a single analytical table
- converted date fields to datetime format
- inspected and handled missing values

### Exploratory Data Analysis (EDA)
- analyzed weekly sales trends over time
- compared holiday and non-holiday sales
- examined monthly seasonality
- identified top-performing stores

### Feature Engineering
- created time-based features
- added lag variables
- built rolling averages
- encoded categorical variables

### Modeling
- model used: Random Forest Regressor
- applied a time-based train/test split to simulate real forecasting conditions

### Evaluation

| Metric | Value |
|--------|------:|
| MAE    | 1,567 |
| RMSE   | 3,341 |
| MAPE   | 15.67% |

## Key Insights

- weekly sales show strong seasonality
- lag features significantly improve predictive performance
- external variables contribute to forecasting accuracy
- a small number of stores account for a large share of total sales

## Tech Stack

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- Jupyter Notebook

## How to Run

1. Clone the repository
2. Download the dataset from Kaggle
3. Place the files inside the `data/` folder
4. Run the notebook

## Future Improvements
- hyperparameter tuning
- testing boosted tree models such as XGBoost or LightGBM
- adding promotion-related variables
- deploying the project as a simple dashboard or app
