# Machine Learning Case Studies

This repository contains two practical Machine Learning case studies
implemented using Python and Google Colab.

The projects focus on applying Machine Learning techniques to real-world
classification problems, including healthcare prediction and financial fraud
detection.

---

## 📚 Case Studies

### 1. Hospital Readmission Prediction

**Objective:**  
Predict whether a patient is likely to be readmitted to the hospital within
30 days.

**Model Used:**
- Logistic Regression
- L2 Regularization

**Key Steps:**
- Data preprocessing
- Missing value handling
- Feature encoding
- Train-test split
- Class imbalance handling using class weights
- Model training
- ROC-AUC evaluation
- Classification report
- Confusion matrix
- ROC curve
- False Positive vs False Negative analysis

**Dataset:**
Diabetes 130-US Hospitals for Years 1999-2008

---

### 2. Credit Card Fraud Detection

**Objective:**  
Detect fraudulent credit card transactions from legitimate transactions.

**Model Used:**
- XGBoost

**Key Steps:**
- Data exploration
- Class imbalance analysis
- Train-test split
- SMOTE for minority-class oversampling
- XGBoost model training
- ROC-AUC evaluation
- Precision, Recall and F1-score
- Confusion matrix
- Decision threshold tuning
- Feature importance analysis

---

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Imbalanced-learn
- Matplotlib
- Google Colab

---

## 📁 Repository Structure

```text
ML-Case-Studies/
│
├── CASESTUDY1MLE
│
├── credit_card_fraud.ipynb
│
└── README.md
