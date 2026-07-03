# Loan Approval Prediction using Machine Learning

## Project Overview

This project develops a machine learning model to predict whether a loan application will be approved. The project follows the **CRISP-DM (Cross-Industry Standard Process for Data Mining)** methodology, covering business understanding, data preparation, modeling, evaluation, and business recommendations.

The goal is to support financial institutions by providing a reliable decision-support tool that improves the efficiency and consistency of loan approval decisions.
## Business Problem

Financial institutions receive thousands of loan applications every year. Manual evaluation can be time-consuming and inconsistent, increasing the risk of poor lending decisions.

This project aims to build a predictive model that helps identify whether a loan application is likely to be approved based on applicant financial and demographic information.
## Dataset

The dataset was obtained from Kaggle and modified for this project to include realistic data quality challenges such as missing values.

### Dataset Summary

- **Records:** 20,000 loan applications
- **Features:** 35
- **Target Variable:** `LoanApproved`

The dataset contains information such as:

- Applicant demographics
- Employment information
- Credit history
- Financial information
- Loan characteristics
- Risk assessment metrics
## CRISP-DM Workflow

This project follows the CRISP-DM methodology:

1. Business Understanding
2. Data Understanding
3. Data Preparation
4. Modeling
5. Evaluation
6. Business Recommendations

## Machine Learning Models

The following classification algorithms were implemented:

- Logistic Regression
- Random Forest Classifier

## Data Preprocessing

The following preprocessing steps were applied:

- Converted `AnnualIncome` from text to numeric values.
- Identified and handled missing values.
- Separated numerical and categorical features.
- Applied median imputation for numerical variables.
- Applied most f
- Encoded categorical variables using One-Hot Encoding.
- Standardized numerical variables using StandardScaler.
- Built preprocessing pipelines using `Pipeline` and `ColumnTransformer`.



Hyperparameter tuning was performed using **GridSearchCV** with cross-validation to identify the best-performing model.

## Model Evaluation

The models were evaluated using multiple classification metrics to ensure reliable performance.

### Evaluation Metrics

- Accuracy
- Precision
- Recall
- F1-Score
- ROC-AUC

A confusion matrix and ROC curve were also generated to visualize model performance.

## Results

After hyperparameter tuning using GridSearchCV, the best-performing model achieved excellent predictive performance on unseen test data.

The final model was able to accurately distinguish between approved and rejected loan applications while maintaining a strong balance between precision and recall.

Feature importance analysis also identified the variables that contributed most to loan approval decisions.
## Important Features

The model identified several variables that strongly influence loan approval decisions, including:

- Risk Score
- Bankruptcy History
- Interest Rate
- Credit Score
- Debt-to-Income Ratio
- Employment Status
- Monthly Income

These variables are consistent with real-world lending practices and provide valuable insights for decision-makers.

## Business Recommendations

Based on the model results, the following recommendations are proposed:

- Use the model as a decision-support tool during loan approval.
- Prioritize applicants with strong financial profiles.
- Carefully review applicants with previous bankruptcies or high debt-to-income ratios.
- Continuously retrain the model using new loan application data.
- Monitor model performance over time to ensure consistent accuracy.

## Repository Structure

```text
Loan-Approval-Prediction/
│
├── README.md
├── requirements.txt
├── Loan_Approval_Prediction.ipynb
├── loan_approval_dataset.csv
├── images/
│   ├── target_distribution.png
│   ├── correlation_heatmap.png
│   ├── confusion_matrix.png
│   ├── roc_curve.png
│   └── feature_importance.png
└── .gitignore
```
## Installation

Clone the repository:

```bash
git clone https://github.com/your-username/Loan-Approval-Prediction.git
```

Navigate to the project folder:

```bash
cd Loan-Approval-Prediction
```

Install the required packages:

```bash
pip install -r requirements.txt
```

Launch Jupyter Notebook:

```bash
jupyter notebook
```

## Author

### mohamed hassan

- Mount Kenya University
- BSc Computer Science
- MBA (Ongoing)
- Data science – Moringa School

Feel free to connect or explore my other data science projects on GitHub.