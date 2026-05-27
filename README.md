# Explainable AI for Credit Card Fraud Detection

A Machine Learning and Explainable AI (XAI) based system for detecting fraudulent credit card transactions using ensemble learning, SMOTE balancing, and interpretable AI techniques like SHAP and LIME.

---

## Description

This project focuses on building an accurate and interpretable fraud detection system for credit card transactions. Since fraudulent transactions represent less than 0.2% of all transactions, detecting fraud is highly challenging due to extreme class imbalance.

The system combines:

- Machine Learning
- Ensemble Learning
- SMOTE Resampling
- Threshold Optimization
- Explainable AI (XAI)

to create a robust fraud detection pipeline capable of identifying fraudulent activities while maintaining transparency and interpretability.

---

## Features

- Credit card fraud detection using Machine Learning
- Handles highly imbalanced datasets using SMOTE
- Stacked ensemble learning architecture
- Threshold optimization using F1-score
- Explainable AI integration
- SHAP and LIME interpretability support
- Fraud probability prediction
- Confusion matrix visualization
- Model persistence using Joblib

---

## Tech Stack

- Python
- Scikit-learn
- XGBoost
- Pandas
- NumPy
- Matplotlib
- Seaborn
- Imbalanced-learn (SMOTE)
- SHAP
- LIME
- Joblib

---

## Dataset Information

The dataset contains:

- 284,807 transactions
- 31 features
- PCA-transformed anonymized variables (V1–V28)
- Transaction Time
- Transaction Amount
- Target Variable:
  - 0 = Legitimate
  - 1 = Fraudulent

### Dataset Challenges

- 99.83% legitimate transactions
- 0.17% fraudulent transactions
- Severe class imbalance

---

## Machine Learning Pipeline

1. Data Loading
2. Feature Scaling
3. Train-Test Split
4. SMOTE Oversampling
5. Model Training
6. Stacked Ensemble Learning
7. Threshold Optimization
8. Model Evaluation
9. Explainable AI Analysis

---

## Models Used

### Base Models

- Logistic Regression
- Random Forest
- XGBoost

### Meta Learner

- Logistic Regression

### Ensemble Method

- Stacking Classifier

---

## Preprocessing Steps

### Feature Scaling

- StandardScaler applied to:
  - Time
  - Amount

### Train-Test Split

- 80% Training
- 20% Testing
- Stratified sampling

### Handling Class Imbalance

SMOTE was used to synthetically balance fraudulent transactions in the training dataset.

---

## Explainable AI (XAI)

### SHAP

Used for:

- Global feature importance
- Local prediction explanations
- Model transparency

### Dataset Link
https://drive.google.com/file/d/1nScXg6ZwmNOuW2Y3J9eYFcpDiwVf5VVX/view?usp=drive_link

---
### LIME

Used for:

- Transaction-level interpretability
- Local explanation generation
- Understanding prediction behavior

---

## Model Performance

| Metric | Score |
|---|---|
| Accuracy | 0.999 |
| Precision | 0.927 |
| Recall | 0.776 |
| F1-Score | 0.844 |
| ROC-AUC | 0.945 |

---


