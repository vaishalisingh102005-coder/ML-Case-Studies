# Credit Card Fraud Detection

## 📌 Problem Statement

Credit card fraud detection is a binary classification problem where the
objective is to identify fraudulent transactions from legitimate transactions.

The dataset is highly imbalanced because fraudulent transactions represent
only a small portion of all transactions.

## 🎯 Objective

Build a Machine Learning model that can identify fraudulent credit card
transactions while handling severe class imbalance.

The model predicts:

- `0` → Legitimate transaction
- `1` → Fraudulent transaction

## 📊 Dataset

The project uses a Credit Card Fraud Detection dataset containing transaction
features and a binary `Class` target.

The dataset contains anonymized numerical features along with transaction
amount information.

## 🧹 Data Preprocessing

The following steps were performed:

1. Loaded the dataset using Pandas.
2. Checked dataset shape and missing values.
3. Analyzed the distribution of legitimate and fraudulent transactions.
4. Separated features (`X`) and target (`y`).
5. Split the data into training and testing sets using stratification.
6. Applied SMOTE only to the training data to handle class imbalance.

## 🤖 Machine Learning Model

### XGBoost

XGBoost was used as the main classification algorithm.

The model was trained on the SMOTE-balanced training dataset and evaluated on
the original test dataset.

## ⚖️ Handling Class Imbalance

SMOTE (Synthetic Minority Over-sampling Technique) was used to increase the
representation of the minority fraud class in the training data.

The test dataset was kept unchanged for evaluation.

## 📈 Evaluation Metrics

The model was evaluated using:

- ROC-AUC
- Precision
- Recall
- F1-score
- Confusion Matrix

## 🎚️ Decision Threshold Tuning

Different probability thresholds were tested:

- 0.1
- 0.2
- 0.3
- 0.4
- 0.5

Changing the threshold allows the model to trade off between precision and
recall depending on the requirements of the fraud detection system.

## 🔍 Feature Importance

XGBoost feature importance was used to identify the features that contributed
most to the model's predictions.

A bar chart of the top 15 features was generated.

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- XGBoost
- Imbalanced-learn
- Matplotlib
- Google Colab

## 📁 Files

- `credit_card_fraud.ipynb` — Complete Google Colab notebook
- `README.md` — Project documentation

## 👩‍💻 Author

Vaishali Singh
