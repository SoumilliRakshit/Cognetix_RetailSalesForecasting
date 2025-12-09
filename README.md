# Retail Sales Forecasting

## Overview
This project focuses on analyzing retail sales data to identify **seasonal trends** and forecast future sales using Python. The goal is to help businesses plan inventory, optimize restocking, and make data-driven decisions.

The dataset is loaded directly from **Kaggle**, and the workflow includes data cleaning, time-series analysis, forecasting, and visualization.

## Dataset
Dataset used: [Retail Dataset by manjeetsingh on Kaggle](https://www.kaggle.com/datasets/manjeetsingh/retaildataset)

**Key Columns:**
- Date / Week (time variable)
- Weekly Sales (target variable)
- Additional columns may include store, product category, etc.

## Features
- **Data Cleaning:** Automatic detection of date and sales columns, handling missing values  
- **Time-Series Analysis:** Trend, seasonality, and pattern analysis  
- **Forecasting:** Holt-Winters exponential smoothing to predict future sales  
- **Visualization:** Line charts comparing actual vs forecasted sales  
- **Inventory Recommendations:** Basic rules for stock adjustments based on forecast  

## How to Run
1. Clone the repository.  
2. Open the notebook in **Google Colab**.  
3. Set your Kaggle API credentials (`KAGGLE_USERNAME` and `KAGGLE_KEY`).  
4. Run all cells — the dataset will be downloaded, analyzed, and forecasts will be generated.

## Libraries Used
- pandas  
- matplotlib  
- statsmodels  
- The seasonal decomposition step is safe for datasets with sufficient observations; otherwise, it is skipped to prevent errors.
- Forecasting is performed even on smaller datasets using Holt-Winters smoothing.
