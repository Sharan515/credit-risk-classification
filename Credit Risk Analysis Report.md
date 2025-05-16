# Module 20 Challenge 

## Overview of the Analysis

The purpose of this analysis is to build and evaluate machine learning models to predict loan status (loan_status) based on financial indicators such as loan size, interest rate, borrower income, debt-to-income ratio, and other relevant metrics. The primary goal is to determine whether a loan is healthy (0) or high-risk (1).

# Data Summary:
- The dataset contains financial variables relevant to lending decisions.
- The target variable is loan_status, where:
- 0 represents healthy loans.
- 1 represents high-risk loans.
- - Feature distribution and balance checks were performed using value_counts() to understand class distributions.

# Machine Learning Process:
- Data Preprocessing:
- Handling missing values (if applicable).
- Feature selection and scaling where necessary.
- Model Selection:
- Logistic Regression was chosen as the primary classification model.
- Alternative models may include Random Forest or Support Vector Machine (SVM).
- Training & Evaluation:
- Train-test split to evaluate performance.
- Metrics used: accuracy, precision, recall, and F1-score.

# Results
Machine Learning Model 1: Logistic Regression
- Accuracy: 99%
- Precision:
- Healthy Loans (0): 1.00
- High-Risk Loans (1): 0.84
- Recall:
- Healthy Loans (0): 0.99
- High-Risk Loans (1): 0.94
- F1-Score:
- Healthy Loans (0): 1.00
- High-Risk Loans (1): 0.89

# Summary & Recommendation
- Best Performing Model: Logistic Regression achieves high accuracy (99%) and strong precision/recall scores.
- Key Considerations:
- If the goal is to minimize false negatives (i.e., catch all risky loans), recall for 1 is 0.94, which is strong.
- If false positives matter (avoiding unnecessary loan rejection), the precision of 1 (0.84) suggests there is room for improvement.

# Final Recommendation:
Logistic Regression appears effective for predicting loan status, particularly in identifying high-risk loans with good recall. If optimizing for precision is crucial, further tuning or trying models like Random Forest may be beneficial



