# Telco_Customer_Churn_Prediction_Using_ML
Developed a Random Forest model to predict customer churn using Python. Preprocessed data, encoded categorical variables, handled class imbalance with SMOTE, and trained multiple models. Key insights: contract type, tenure, charges, and tech support impact churn.

## Project Overview
This project demonstrates a machine learning approach to predict customer churn for a telecom company. By analyzing customer data, preprocessing it, and training predictive models, we can identify customers likely to leave the service. This enables businesses to implement targeted retention strategies.

---

## Problem Statement
Customer churn is the phenomenon where customers stop using a company’s service. Predicting churn helps companies reduce revenue loss by proactively retaining customers.

**Goal:** Predict whether a customer will churn using historical data, and extract insights to improve retention strategies.

---

## Dataset
- The dataset contains information about customers, their account details, and services used.  
- Key features include:
  - Customer demographics: Gender, Senior Citizen, Partner, Dependents  
  - Account details: Tenure, Contract, Payment Method, MonthlyCharges, TotalCharges  
  - Service usage: Phone Service, Multiple Lines, Internet Service, Online Security, Tech Support, Streaming Services  
- Target variable: `Churn` (Yes / No)

---

## Tools & Technologies
- Python 3.x  
- Libraries: `pandas`, `numpy`, `scikit-learn`, `imbalanced-learn`, `matplotlib`, `seaborn`, `pickle`  

---

## Project Workflow
1. **Data Loading**: Load the raw customer dataset.  
2. **Data Preprocessing**:
   - Handle missing values and convert data types
   - Encode all categorical variables using `LabelEncoder`
   - Scale numerical features
   - Handle class imbalance using **SMOTE**
   - Save preprocessed data (`customer_churn_preprocessed.csv`)
3. **Exploratory Data Analysis (EDA)**:
   - Univariate and bivariate analysis to identify patterns
   - Insights on features most affecting churn
4. **Model Training**:
   - Models tested: Decision Tree, Random Forest, XGBoost
   - Train-Test split (80:20)
   - Train models on SMOTE-resampled data
5. **Model Evaluation**:
   - Metrics: Accuracy, Precision, Recall, F1-score, Confusion Matrix
   - Random Forest selected as the final model for best performance
6. **Deployment / Prediction**:
   - Random Forest model saved using `pickle`
   - Can predict churn on new/unseen data

---
Author

Fahiz Mohammed  – 
LinkedIn:www.linkedin.com/in/fahiz-mohammed-68130421b
