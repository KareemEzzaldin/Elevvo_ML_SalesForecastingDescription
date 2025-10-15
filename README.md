# Sales Forecasting

Predict weekly store sales using linear regression and lag-based features.

---

## Overview

This project builds a time-series regression model to forecast weekly sales for retail stores.  
It merges multiple datasets, creates lag features, and trains a linear regression model to predict future sales.  
Model performance is evaluated using **Root Mean Squared Error (RMSE)**.

---

## Steps

- Load and merge datasets (`train.csv`, `features.csv`, `stores.csv`)  
- Convert `Date` columns to datetime format  
- Extract year and week from the date  
- Aggregate weekly sales per store  
- Create lag features for previous week sales  
- Train Linear Regression model  
- Evaluate using RMSE  
- Visualize actual vs predicted sales  

---

## Dataset

**Files:**

- `train.csv` – historical weekly sales per store  
- `features.csv` – includes holiday and temperature data  
- `stores.csv` – contains store metadata such as type and size  

Key columns:

- `Store`  
- `Date`  
- `Weekly_Sales`  
- `IsHoliday`  
- `Type`, `Size`

Target variable: **Weekly_Sales**

---

## Requirements

Install dependencies:

```bash
pip install pandas numpy scikit-learn matplotlib
