# Milestone 1: Predictive Analytics for Customer Churn

## Project Overview

This project develops a predictive analytics model to identify customers who are likely to churn from a subscription-based telecommunications service. The main goal is to use tabular customer data to train and evaluate machine learning models that can support customer retention decisions.

## Dataset

The dataset used in this project is the Telco Customer Churn dataset. It contains customer demographic information, service usage, account information, and historical churn labels.

The target variable is `Churn_Value`, which indicates whether a customer has churned or not.

## Project Workflow

The notebook follows the required workflow:

1. Import libraries
2. Load dataset
3. Data cleaning
4. Exploratory Data Analysis
5. Feature engineering
6. Train-test split and preprocessing
7. Model training
8. Model evaluation
9. Conclusion

## Data Cleaning

The data cleaning process included checking missing values, converting `Total_Charges` into a numerical format, checking duplicated records, and removing columns that could cause data leakage, such as `Churn_Reason`, `Churn_Label`, and `Churn_Score`.

## Feature Engineering

New features were created to improve model performance and better represent customer behaviour:

* `tenure_group`
* `total_services`
* `avg_charge_per_month`

## Models Used

Three machine learning models were trained and compared:

* Logistic Regression
* Decision Tree
* Random Forest

## Evaluation Metrics

The models were evaluated using:

* Accuracy
* Precision
* Recall
* F1-score
* ROC-AUC

F1-score was used to select the best-performing model because churn prediction requires balancing precision and recall.

## Conclusion

Based on the evaluation results, Random Forest was selected as the best-performing model using F1-score. In a real business environment, this model could help a company identify high-risk customers earlier and design retention strategies such as personalised offers, improved customer support, or loyalty discounts.

## How to Run

1. Open the notebook file in Google Colab.
2. Upload the dataset file when prompted.
3. Run all cells from top to bottom.
4. Review the evaluation results and conclusion.
