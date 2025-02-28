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
