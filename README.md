📊 Customer Churn Prediction & Analysis Project

📌 Project Overview
This project focuses on analyzing customer churn behavior and building a machine learning model to predict customers who are likely to churn. The goal is to help businesses identify high‑risk customers and take proactive retention actions.

The project was completed in three phases:

1. SQL Data Preparation
2. Machine Learning Modeling (Python)
3. Visualization & Business Dashboard (Power BI)

🗂 Dataset Description
The dataset contains customer demographic details, service usage information, billing details, and churn status.

Key Columns:
1.tenure
2.monthlycharges
3.totalcharges
4.contract
5.internetservice
6.paymentmethod
7.seniorcitizen
8.churn_new (Target Variable: 1 = Churn, 0 = No Churn)
9.predicted_probability (Model Output)

🛠 Phase 1 – SQL Data Preparation
Performed:
Removed unnecessary columns (e.g., customerID)
Converted churn column to numeric (0/1)
Ensured correct data types
Cleaned null values
Exported final dataset for modeling
Output:
telco_customer_churn_clean.csv

🤖 Phase 2 – Machine Learning (Python)
Steps Performed:
Data Loading & Inspection
Feature Encoding (One-Hot Encoding)
Train-Test Split (80/20 with stratification)
Logistic Regression Model Training
Model Evaluation
Threshold Optimization
Feature Importance Analysis

📈 Model Performance
Model Used: Logistic Regression
ROC-AUC Score: 0.8426
Accuracy: 80%
Recall (Churn Class):
Default Threshold (0.5): 56%
Optimized Threshold (0.3): 76%
Random Forest was also tested (ROC-AUC = 0.8253), but Logistic Regression performed better.

🔍 Key Churn Drivers Identified
Top features increasing churn probability:
Fiber Optic Internet
Electronic Check Payment Method
Paperless Billing
Multiple Lines
Streaming Services

📊 Phase 3 – Power BI Dashboard
The Power BI dashboard includes:

🔹 KPI Cards
Total Customers
Total Churn Customers
Churn Rate %
High Risk Customers
High Risk %

🔹 Visual Analysis
Churn by Contract Type
Churn by Internet Service
Churn by Payment Method
Tenure vs Churn
High Risk Customer Segmentation

🔹 Risk Classification
Customers are categorized as:
High Risk (Probability > 0.3)
Low Risk

🎯 Business Insights

Customers using Fiber Optic service show higher churn probability.
Electronic Check users are more likely to churn.
Lower tenure customers have higher churn rates.
Model detects 76% of potential churners using optimized threshold.

🚀 Business Recommendation

Target High-Risk customers with retention campaigns.
Offer loyalty discounts for Fiber Optic users.
Promote automatic payment methods.
Focus on early engagement for new customers.

👥Team Members & Roles

Member 1 – SQL Developer  [Trived7]
Data cleaning, query writing, database management
Member 2 – Python & ML Developer [ArunKusumanchi]
EDA, feature engineering, model building
Member 3 – Power BI Developer [Sumedhapalla] [TEAM LEADER]
Dashboard design, DAX measures, visualization

🏁 Conclusion 🚀

This project successfully built an end‑to‑end churn prediction system using:
SQL for Data Cleaning
Python for Machine Learning
Power BI for Visualization
The model provides actionable insights and supports data‑driven customer retention strategies
