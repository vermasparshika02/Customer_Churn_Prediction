# Credit Card Default Risk Prediction

## Project Overview
This project focuses on analysing credit card customer data and predicting the likelihood of future payment default using Machine Learning.

The objective is to identify patterns in customer repayment behaviour, explore factors associated with default risk, and compare classification models to support data-driven credit risk assessment.

## Dataset
- **Source:** [UCI Machine Learning Repository – Default of Credit Card Clients](https://archive.ics.uci.edu/dataset/350/default+of+credit+card+clients)
- **Records:** 30,000 customers
- **Features:** 23 input variables
- **Target:** Default payment next month (0 = No Default, 1 = Default)

The dataset includes customer demographics, credit limits, repayment status, bill amounts, and previous payment amounts.

## Tools & Technologies
- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Scikit-learn
- Google Colab

## Project Workflow

1. **Data Cleaning:** Checked dataset structure, data types, missing values, and removed the customer ID and original header row.
2. **Exploratory Data Analysis:** Analysed customer demographics, age groups, repayment status, credit limits, and default distribution.
3. **Data Preprocessing:** Separated input features and target variable, performed stratified train-test splitting, and applied feature scaling for Logistic Regression.
4. **Model Development:** Implemented Logistic Regression and Random Forest classifiers.
5. **Model Evaluation:** Compared models using accuracy, precision, recall, F1-score, and ROC-AUC.

## Model Performance

| Metric | Logistic Regression | Random Forest |
|---|---:|---:|
| Accuracy | 67.97% | 79% |
| Default Precision | 37% | 53% |
| Default Recall | 62% | 55% |
| Default F1-score | 0.46 | 0.54 |
| ROC-AUC | 0.7081 | 0.7731 |

Random Forest achieved better overall performance across most evaluation metrics, while Logistic Regression achieved higher recall for the default class.

## Key Findings
- Approximately 22.12% of customers in the dataset defaulted.
- Repayment status showed a strong association with future default.
- Default rates varied across customer age groups.
- Random Forest performed better in overall classification and discrimination, while Logistic Regression identified a greater proportion of actual defaulters at the default threshold.

## Future Improvements
- Feature importance analysis and model interpretability.
- Model optimisation and threshold tuning.
- Interactive Power BI dashboard.
- Business recommendations based on credit risk patterns.

## Disclaimer
This project is for educational and analytical purposes. Model predictions should not be used as the sole basis for real-world lending or credit decisions.
