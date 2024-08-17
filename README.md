# Telecom Customer Churn Analysis

This project performs Exploratory Data Analysis (EDA) on a telecom customer churn dataset to understand factors influencing customer churn.

## Data Loading and Initial Exploration

1. Imported necessary libraries: pandas, numpy, matplotlib, seaborn, statsmodels
2. Loaded data from "high_churn_list_model.csv"
3. Examined basic statistics and data types of categorical and numerical variables

## Churn Analysis

1. Calculated overall churn rate
2. Analyzed churn rates by demographic factors (Married, Gender)
3. Visualized age distribution across gender and marital status
4. Plotted distributions of key numerical variables (Total Revenue, Total Charges, Tenure)

## Feature Analysis

1. Examined correlations between numerical variables and churn
2. Visualized distributions and counts of various categorical variables
3. Analyzed churn rates across different contract types, offers, and internet types

## Logistic Regression Modeling

### Model 1: Numerical Variables
- Built a logistic regression model using key numerical variables
- Analyzed coefficients and p-values to identify significant predictors of churn

### Model 2: Binary Categorical Variables
- Created a model using binary categorical variables (Gender, Married, PhoneService, InternetService, PaperlessBilling)
- Calculated odds ratios to interpret the impact of these variables on churn

### Model 3: Multi-category Variables
- Utilized one-hot encoding for multi-category variables (Offer, InternetType, Contract, PaymentMethod)
- Built separate models for each category to understand their impact on churn

## Key Findings

1. Tenure, number of referrals, and total charges are negatively correlated with churn
2. Monthly charges and age show positive correlation with churn
3. Married customers and those with phone service are less likely to churn
4. Fiber optic internet users and those on month-to-month contracts have higher churn rates
5. Certain offers (e.g., Offer A and B) are associated with lower churn rates

This EDA provides insights into factors influencing customer churn, which can be used to develop retention strategies and improve customer satisfaction.
