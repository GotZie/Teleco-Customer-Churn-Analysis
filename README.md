# Telco Customer Churn Prediction

## Overview

This project develops and evaluates multiple machine learning models to predict customer churn for a telecommunications company. The objective is to identify customers at risk of leaving and provide actionable insights that support targeted retention strategies.

The workflow combines data cleaning, exploratory data analysis (EDA), feature engineering, model benchmarking, threshold optimization, and business interpretation.

## Problem Statement

Customer churn directly impacts recurring revenue. The goal is to accurately identify customers likely to churn so the business can proactively intervene while balancing the cost of retention campaigns against missed churners.

## Dataset Summary

**Dataset:** Telco Customer Churn

**Target Variable:** `Churn`

**Class Distribution:** Approximately 74% non-churn, 26% churn.

**Feature Categories**
- Customer demographics
- Account information
- Services subscribed
- Contract details
- Billing and payment information

## Repository Structure

```text
├── data/
├── notebooks/
├── visuals/
├── README.md
├── requirements.txt
└── LICENSE
```

## Approach

### 1. Data Cleaning
- Corrected data types
- Treated missing `TotalCharges`
- Encoded categorical variables

### 2. Exploratory Data Analysis
- Churn distribution
- Numerical and categorical analysis
- Correlation analysis
- Business insight generation

### 3. Feature Engineering
- One-hot encoding
- Cramer's V analysis
- Removed redundant features
- Threshold optimization

### 4. Machine Learning
Models evaluated:
- Logistic Regression
- Random Forest
- XGBoost
- LightGBM
- K-Nearest Neighbours

Evaluation metrics:
- Precision
- Recall
- F1-Score
- ROC-AUC

## Key Findings

- Tenure, MonthlyCharges, and TotalCharges were consistently the strongest predictors of churn.
- Customers with shorter tenure and higher monthly charges were more likely to churn.
- Logistic Regression achieved the highest optimized F1-Score.
- LightGBM delivered the strongest balanced performance before threshold optimization.
- Random Forest achieved the highest recall after threshold optimization.

## Business Recommendations

- Prioritize retention campaigns for new customers.
- Target high monthly charge customers with personalized offers.
- Encourage longer-term contracts.
- Monitor payment methods associated with elevated churn risk.

## Technologies Used

- Python
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Scikit-learn
- XGBoost
- LightGBM

## Author

**CHIGOZIE OKONKWO**

Electrical & Electronics Engineer | Data Scientist | Energy & Business Analytics
