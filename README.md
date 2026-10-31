# Predicting Customer Churn Using Machine Learning

## Project Overview

This project investigates whether machine learning can predict customer churn in a telecommunications company using customer demographic, service and account information.

The project is part of the CT4101 Machine Learning Portfolio Project at the University of Galway.

## Dataset

The project uses the IBM Telco Customer Churn dataset, containing 7,043 customer records and 21 columns.

Dataset source: https://github.com/IBM/telco-customer-churn-on-icp4d

The target variable is `Churn`:
- 0 = Customer stayed
- 1 = Customer left

The customer ID is excluded from the predictive features.

## Milestone 2 — Data Preparation and Baseline

The following work has been completed:

- Loaded and explored the dataset.
- Checked data types and missing values.
- Checked for duplicate records.
- Examined the churn distribution and numerical outliers.
- Converted `TotalCharges` into a numeric column.
- Identified 11 missing `TotalCharges` values.
- Converted the target variable into 0 and 1.
- Created an 80/20 stratified training and testing split.
- Defined a preprocessing pipeline for numerical and categorical features.
- Trained and evaluated a majority-class Dummy Classifier.

## Baseline Model Results

| Metric | Result |
|---|---|
| Accuracy | 0.7346 |
| Precision | 0.0000 |
| Recall | 0.0000 |
| F1-score | 0.0000 |
| ROC-AUC | 0.5000 |

The baseline model predicts that every customer will stay. Although it achieves approximately 73.46% accuracy, it fails to identify customers who actually churn.

## Running the Project

1. Install the packages listed in `requirements.txt`.
2. Open `customer_churn_milestone2.ipynb` in Google Colab or Jupyter Notebook.
3. Run the notebook cells in order from top to bottom.
4. The notebook downloads the dataset from the IBM GitHub source and generates the baseline evaluation results.

An internet connection is required to download the dataset.

## Next Steps

In Milestone 3, Logistic Regression, Decision Tree and Random Forest models will be trained and compared against the baseline.

## Assistance Declaration

Generative AI (ChatGPT) was used to assist with code development, explanations, project documentation and interpretation of results. The project workflow and outputs are being reviewed and tested by the student.
