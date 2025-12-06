# Customer Churn Prediction – End-to-End ML Pipeline

This project implements a complete machine learning pipeline to predict customer churn using the Telco Customer Churn dataset. It covers data preprocessing, EDA, feature engineering, imbalance handling, model training, and performance evaluation.

---

## 1. Project Objective
Build a predictive model that identifies whether a customer is likely to churn, enabling data-driven retention strategies.

---

## 2. Dataset
**File:** `Telco_customer_churn.xlsx`  
**Target Variable:** `Churn Value` (0 = No churn, 1 = Churn)

Dataset contains:
- Customer demographics  
- Subscription details  
- Billing information  
- Churn indicators  

---

## 3. Workflow Summary

### ✔ Data Cleaning
- Converted `Total Charges` to numeric  
- Removed high-missing columns  
- Dropped irrelevant starting columns  
- Handled missing values  
- Removed outliers using IQR  

### ✔ Exploratory Data Analysis (EDA)
- Churn distribution  
- Numeric feature distributions  
- Tenure vs Churn  
- Contract type vs Churn  
- Correlation heatmap  

### ✔ Feature Engineering
- One-Hot Encoding for categorical features  
- Standard scaling for numerical features  
- Class imbalance handled using **SMOTE**

### ✔ Modeling
Models trained:
- Logistic Regression  
- Random Forest  
- XGBoost  

Evaluated using:
- Accuracy  
- Precision  
- Recall  
- F1-Score  
- Confusion Matrix  

### ✔ Model Saving
```
joblib.dump(model, "best_churn_model.pkl")
```

---

## 4. Repository Structure
```
├── Customer_Churn_prediction.ipynb
├── Telco_customer_churn.xlsx
└── README.md
```

---

## 5. Key Outcomes
- Cleaned and transformed dataset  
- Balanced training data using SMOTE  
- Compared multiple ML models  
- Exported best-performing model  
