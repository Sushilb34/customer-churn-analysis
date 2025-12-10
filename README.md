# customer-churn-analysis
End-to-end Customer Churn Prediction using EDA, Segmentation, and Logistic Regression

This project focuses on understanding customer churn behavior using Exploratory Data Analysis (EDA), customer segmentation, and building a predictive model using Logistic Regression. The objective is to identify key churn drivers, segment customers, and predict which customers are at risk of leaving.
📁 Dataset Overview
-This dataset contains customer information from a telecom company.
-Each row represents a customer, including:
-Demographics: gender, senior citizen, partner, dependents
-Account Information: tenure, contract, payment method
-Services: phone, internet, streaming, tech support
-Charges: monthly charges, total charges
-Target Variable: Churn (Yes/No)

✅ Task 1: Data Cleaning & Preprocessing

✔ Checked for missing values
✔ Converted data types (e.g., TotalCharges → numeric)
✔ Encoded categorical variables using One-Hot Encoding
✔ Standardized and prepared the dataset for modeling
This step ensures the dataset is clean and ready for analysis.

Task 2: Exploratory Data Analysis (EDA)
Visual insights generated:
Overall churn rate
-Churn by:
-gender
-partner status
-dependents
-contract type
-payment method
Tenure distribution and its impact on churn.

 Task 3: Customer Segmentation

Customers were segmented using:
-Tenure groups
-Monthly charge levels
-Contract types
Then churn rates were analyzed in each segment.

 Findings:
New customers (low tenure) churn more.
High-paying customers with Month-to-Month contracts are the highest-risk group.
Long-term contract customers are the lowest-risk group.
This helps identify high-value, high-risk customers that need attention.

Task 4: Churn Prediction Model (Logistic Regression)

Steps:
Train-test split
Feature scaling
Train Logistic Regression
Model evaluation:
  -Accuracy
  -Precision
  -Recall
  -F1-Score
Confusion Matrix

 Model Results:
Accuracy: 0.8038
Precision: 0.6476
Recall: 0.5749
F1-Score: 0.6091
ROC AUC: 0.8356
Confusion Matrix:
 [[916 117]
 [159 215]]

 Classification Report:
               precision    recall  f1-score   support

           0       0.85      0.89      0.87      1033
           1       0.65      0.57      0.61       374

    accuracy                           0.80      1407
   macro avg       0.75      0.73      0.74      1407
weighted avg       0.80      0.80      0.80      1407

# Interpretation
  The logistic regression model predicts which customers are likely to churn, allowing the company to take preventive actions.

  This project provides:
A complete churn analysis pipeline.
Clear demographic and behavioral insights.
Customer segmentation for strategy.
A working machine learning model to predict churn.
