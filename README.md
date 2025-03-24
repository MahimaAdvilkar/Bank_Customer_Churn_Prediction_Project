# 🧠 Customer Churn Prediction Using Machine Learning

**Prepared by:** Mahima Advilkar  
**Role:** Data Analyst  
**Domain:** Predictive Modeling | Banking Analytics  
**Tools Used:** Python, scikit-learn, pandas, seaborn, matplotlib

## 📌 Project Objective

This project focuses on predicting customer churn in a banking environment using supervised machine learning. By identifying key churn drivers, the model helps banks take action to retain valuable customers.

## 📂 Dataset

- **Source:** Synthetic banking data from a European bank
- **Records:** 10,000
- **Target Variable:** `Exited` (1 = churned, 0 = retained)

### Features include:
- **Demographics:** Geography, Gender, Age
- **Behavior:** CreditScore, Tenure, Balance, Products, Activity
- **Financials:** EstimatedSalary

## 🔍 Exploratory Data Analysis (EDA)

- Churn rate ≈ 20%
- Older, inactive customers churn more
- High balance without engagement is a churn signal
- German customers showed higher churn

## 🛠 Feature Engineering & Preprocessing

- Encoding (Label, One-Hot)
- Engineered features like `BalanceToSalaryRatio`, `ProductUsage`, `BalanceZero`
- Scaling with StandardScaler

## 🤖 Models Trained

| Model                  | Accuracy |
|------------------------|----------|
| Gradient Boosting      | 86.45%   |
| Random Forest          | 86.25%   |
| Logistic Regression    | 80.45%   |
| K-Nearest Neighbors    | 79.85%   |
| SVM (Linear Kernel)    | 79.60%   |

### 📈 Evaluation Metrics
- Accuracy
- Precision
- Recall
- F1-Score
- Confusion Matrix

## 🔍 Key Insights

- Age and activity levels are strong churn predictors
- Multi-product customers are more likely to stay
- Engagement levels (IsActiveMember) drive retention

## 💡 Business Recommendations

- Segment high-risk customers (older, inactive)
- Launch engagement and product adoption campaigns
- Monitor customer activity regularly

## 🚀 Deployment Plan

- Integrate model into CRM
- Weekly churn scoring dashboard
- Set up churn alert thresholds
- Plan for quarterly retraining

## 🛣 Next Steps

- GridSearchCV for hyperparameter tuning
- SMOTE/class weights for balancing
- Wrap model into a Flask/FastAPI app
- Monitor for drift and retrain periodically

## 📎 Files Included

- `Customer_Churn_Prediction.ipynb` – Main notebook  
- `Churn_Modelling.csv` – Dataset  
- `Customer_Churn_Report.pdf` – Final report  
- `/images/` – Visuals used in the report (optional)

---

> Feel free to fork, explore, and adapt this project.  
> If you find it helpful, give the repo a ⭐!

