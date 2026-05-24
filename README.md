🚀 Bank Marketing Prediction using Logistic Regression
📌 Project Overview

This project is an end-to-end machine learning classification system built to predict whether a customer will subscribe to a term deposit based on bank marketing data.

It focuses on solving a real-world imbalanced classification problem using Logistic Regression with proper preprocessing, evaluation, and threshold tuning.

📊 Dataset Information
📁 Shape: 41,000 rows × 21 columns
🎯 Target: y (Yes / No subscription)
⚖️ Highly imbalanced dataset
📌 Real-world bank marketing campaign data
🧠 Problem Statement

Predict whether a customer will subscribe to a term deposit using demographic, financial, and campaign-related features.

🔧 Tech Stack
Python 🐍
Pandas & NumPy
Scikit-learn
Matplotlib
Seaborn
⚙️ Project Workflow
1️⃣ Data Preprocessing
Handled missing values and "unknown" entries
Converted categorical variables using One-Hot Encoding
Scaled numerical features using StandardScaler
2️⃣ Feature Engineering
Separated categorical and numerical columns
Applied ColumnTransformer for combined preprocessing
3️⃣ Model Building
Used Logistic Regression
Built using Pipeline to avoid data leakage
Applied class_weight='balanced' for imbalanced dataset handling
4️⃣ Model Evaluation
Accuracy Score
Precision, Recall, F1-Score
Confusion Matrix
ROC-AUC Curve
5️⃣ Threshold Tuning
Used probability outputs (predict_proba)
Optimized decision threshold using ROC curve analysis (Youden’s J statistic)
📊 Model Performance
Metric	Score
Accuracy	80%
Precision	0.31
Recall	0.64
F1 Score	0.42
ROC-AUC	0.78
🧠 Key Insights
Dataset is highly imbalanced, affecting precision
Recall is more important than precision for this business case
Threshold tuning significantly improves model behavior
ROC-AUC shows good class separability (0.78)
🎯 Business Understanding

In this problem:

Missing a potential “YES” customer leads to lost revenue
Therefore, Recall is prioritized over Precision
📈 Key Techniques Used
Logistic Regression
One-Hot Encoding
Feature Scaling
Class Weight Balancing
ROC Curve Analysis
Threshold Optimization
🚀 Results Summary

The model achieves a strong balance between performance metrics with good recall and solid ROC-AUC, making it suitable for real-world marketing prediction scenarios.
