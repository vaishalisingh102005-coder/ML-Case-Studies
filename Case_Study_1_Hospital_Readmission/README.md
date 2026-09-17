# Hospital Readmission Prediction

## 📌 Problem Statement

Hospital readmission within 30 days is an important healthcare problem.
This case study uses Machine Learning to predict whether a patient is likely
to be readmitted to the hospital within 30 days.

The model is trained using patient encounter, diagnosis, medication and
hospital utilization information.

## 🎯 Objective

The main objective is to build a binary classification model that predicts:

- `1` → Patient is readmitted within 30 days
- `0` → Patient is not readmitted within 30 days

## 📊 Dataset

Dataset: Diabetes 130-US Hospitals for Years 1999-2008

The dataset contains hospital encounter records with information such as:

- Patient demographics
- Admission information
- Diagnosis codes
- Number of previous outpatient visits
- Number of emergency visits
- Number of inpatient visits
- Laboratory procedures
- Procedures performed
- Medications
- Length of hospital stay
- Number of diagnoses

## 🧹 Data Preprocessing

The following preprocessing steps were performed:

1. Replaced missing-value indicators with NaN.
2. Removed columns with a very high percentage of missing values.
3. Created a binary target variable for 30-day readmission.
4. Separated numerical and categorical features.
5. Applied median imputation and standardization to numerical features.
6. Applied most-frequent imputation and One-Hot Encoding to categorical features.
7. Used a stratified train-test split.

## 🤖 Machine Learning Model

### Logistic Regression

Logistic Regression was used as the classification algorithm.

L2 regularization was applied to reduce overfitting and improve model
generalization.

Because the dataset is imbalanced, class weights were also used to give
greater importance to the minority class.

## 📈 Evaluation Metrics

The model is evaluated using:

- ROC-AUC
- Precision
- Recall
- F1-score
- Confusion Matrix
- ROC Curve

## 🏥 Clinical Considerations

In a hospital readmission prediction system, false negatives and false
positives can have different consequences.

A false negative means a patient who is actually readmitted within 30 days
was predicted as not being readmitted.

A false positive means a patient who is not readmitted within 30 days was
predicted as being at risk.

The relative cost of these errors should be considered when selecting an
appropriate prediction threshold.

## 📁 Files

- `hospital_readmission.ipynb` — Complete Jupyter/Google Colab notebook
- `README.md` — Project documentation

## 🛠️ Technologies Used

- Python
- Pandas
- NumPy
- Scikit-learn
- Matplotlib
- Google Colab

## 👩‍💻 Author

Vaishali Singh
