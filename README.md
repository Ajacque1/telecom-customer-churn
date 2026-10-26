# Telecommunications Customer Churn Prediction

## Project Overview

This project uses Python and machine learning to analyze telecommunications customer behavior and predict customer churn.

The goal is to identify patterns associated with customer cancellations and explore how predictive analytics could support customer retention strategies.

## Dataset

- **Source:** IBM Telco Customer Churn sample dataset
- **Customer records:** 7,043
- **Variables:** 21
- **Overall churn rate:** 26.54%

## Technologies Used

- Python
- pandas
- Matplotlib
- scikit-learn
- Jupyter Notebook

## Key Findings

**Contract Type:** Month-to-month customers had a churn rate of 42.71%, compared with 11.27% for one-year contracts and 2.83% for two-year contracts.

**Monthly Charges:** Customers who canceled paid an average of $74.44 per month, compared with $61.27 for customers who remained.

## Machine Learning Results

Two classification models were evaluated: Logistic Regression and Random Forest.

| Model | Threshold | Precision | Recall | F1-score |
|---|---|---|---|---|
| Logistic Regression | 40% | 59.95% | 66.04% | 62.85% |
| Random Forest | 30% | 53.50% | 75.67% | 62.68% |

Results reflect validation-set performance.

Logistic Regression was provisionally selected because it achieved a slightly higher F1-score at the evaluated thresholds.

The original test set was examined during exploratory development, so an entirely untouched final test evaluation is not claimed.

## Business Value

The model demonstrates how telecommunications companies could use customer information to identify accounts with elevated cancellation risk.

These predictions could help retention teams prioritize customers for further evaluation and targeted outreach.

## Limitations and Future Improvements

The analysis uses sample data and four predictive features. Future improvements could include additional features, model calibration, independent evaluation, and an interactive dashboard.

## How to Run

Install the dependencies using `pip install -r requirements.txt`, then open `telcom_churn_project.ipynb` in Jupyter Notebook and run the cells in order.