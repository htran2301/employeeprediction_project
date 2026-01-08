# Employee Attrition Prediction – Machine Learning

## 📌 Project Overview
This project builds a supervised machine learning pipeline to predict employee attrition using the IBM HR Analytics dataset (1,470 employees). The goal is to identify employees at risk of leaving and uncover key drivers of attrition to support proactive, data-driven retention strategies.

---

## 🎯 Objectives
- Predict whether an employee will leave or stay
- Address class imbalance in attrition data
- Compare multiple classification models
- Identify key factors contributing to employee turnover

---

## 🗂️ Dataset
- Source: IBM HR Analytics Employee Attrition dataset
- Size: 1,470 employee records
- Features include:
  - Demographics (age, gender, income)
  - Job-related factors (job role, job level, overtime)
  - Satisfaction and work-life balance metrics
- Target variable: Employee Attrition (Yes / No)

---

## 🔄 Project Workflow

### 1. Data Preparation
- Removed constant and non-informative columns
- Encoded categorical variables
- Scaled numerical features using StandardScaler
- Preserved valid outliers representing real employee groups

---

### 2. Exploratory Analysis
- Examined attrition patterns across demographics and job characteristics
- Identified early signals such as lower tenure, lower satisfaction, and overtime

---

### 3. Modeling
Trained and evaluated multiple classification models:
- Logistic Regression
- Decision Tree
- Random Forest
- Support Vector Machine (SVM)
- XGBoost

Addressed class imbalance (only ~16% attrition cases) using:
- Stratified train-test split
- Class weighting
- SMOTE (Synthetic Minority Over-sampling Technique)

---

### 4. Model Evaluation
Models were evaluated using:
- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

Logistic Regression with **SMOTE + hyperparameter tuning** provided the best balance between recall and precision, minimizing false positives while effectively identifying at-risk employees.

---

## 🔑 Key Insights
- Overtime, job level, and total working years are strong predictors of attrition
- Handling class imbalance significantly improves model reliability
- Simpler, interpretable models can outperform complex models in HR use cases

---

## 🧠 Tools & Technologies
- Python
- pandas, NumPy
- scikit-learn
- imbalanced-learn (SMOTE)
- Jupyter Notebook

---

## 📈 Outcome
This project demonstrates how machine learning can be applied to HR analytics to shift from reactive turnover management to proactive retention planning, balancing predictive performance with interpretability for real-world decision-making.

---

## ⚠️ Notes
- Dataset is historical and static
- Results are intended for analytical and educational purposes

Contributors: 
Pouya Khazaeli Pour
Hiba Ashan 
Sumanth 
Mourya

