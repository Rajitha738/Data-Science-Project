# 🏦 Customer Transaction Prediction

## 📌 Problem Statement

This project aims to build a predictive model to help a bank identify which customers are likely to make a transaction in the future. The dataset is anonymized and contains 200 features, along with an `ID_code` and a `target` column where:

- `1` → Customer **will** make a transaction  
- `0` → Customer **will not** make a transaction

---

## 📁 Dataset Information

- **Source:** [Download Dataset](https://d3ilbtxij3aepc.cloudfront.net/projects/CDS-Capstone-Projects/PRCP-1003-CustTransPred.zip)
- **Features:** 200 anonymized features
- **ID_code:** Unique identifier for each customer
- **Target:** Binary label indicating transaction (1) or no transaction (0)

> ⚠️ Due to anonymized features, exploratory data analysis (EDA) was skipped.

---

## 🛠 Tasks Performed

### ✅ Task 1: Data Analysis
- Verified data integrity and balance
- Handled missing values
- Checked target distribution
- Feature scaling using StandardScaler
- Applied train-test split

### ✅ Task 2: Model Building
Built and evaluated the following classification models:
- Logistic Regression (LR)
- Decision Tree (DT)
- XGBoost Classifier (XGB)
- Multi-Layer Perceptron (MLP)

Class imbalance handled using:
- Class weighting
- Synthetic Minority Oversampling Technique (SMOTE)

---

## 📌 Evaluation Metrics Used

- **Accuracy** – Overall correctness of the model
- **Precision** – Correctness of positive predictions
- **Recall** – Ability to find all positive samples
- **F1-Score** – Balance between precision and recall

---

## 🚧 Challenges Faced

- **No feature names**: Unable to perform domain-level feature analysis. Used model-based feature importance instead.
- **High dimensionality**: Dataset had 200 features, leading to increased training time. Regularization and model tuning were key.
- **Class imbalance**: More non-transaction cases. Applied class weighting to improve recall for minority class.
