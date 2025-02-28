# Customer Churn Prediction - Data Insights & Feature Engineering

## 📌 1. Exploratory Data Analysis (EDA)
- `Contract`, `PaperlessBilling`, and `PaymentMethod` significantly impact churn.
- `Tenure` is positively correlated with retention (longer tenure → lower churn).

## 📌 2. Hypothesis Testing Results
| Feature            | Chi-Square p-value | Decision |
|--------------------|------------------|---------|
| Contract Type     | < 0.05 ✅  | Significant |
| Payment Method    | < 0.05 ✅  | Significant |
| Paperless Billing | < 0.05 ✅  | Significant |

## 📌 3. Feature Engineering Plan
- **Categorical Features** → One-Hot Encoding
- **Numerical Features** → StandardScaler
- **Feature Selection** → Drop low-impact features

# Analyses from Feature Engineering
    - First we drop the unnecessary column (Customer ID)
    - Encode Categorical columns
    - Starting off with SeniorCitizen column which was originally int datatype and has unique values[0,1], so do we have to scale?
    - Yes, if we are using any model in future except for tree models , to maintain consistency across models it is good practice to scale it for better convergence and performance of models
    -