# Credit Risk Classification

# Overview of the Analysis
The purpose of this analysis is to evaluate the performance of a machine learning model designed to predict loan statuses as either healthy or high-risk, based on a variety of financial data. This analysis focuses on using a Logistic Regression model to classify loans into two categories:

- 0: Healthy loans
- 1: High-risk loans

The dataset includes variables such as loan size, interest rate, borrower income, and debt-to-income ratio, among others, to help predict whether a loan will default or remain healthy. Specifically, the model was trained to predict the loan_status variable, which indicates whether the loan is likely to default (1) or not (0).

In this analysis, there are few steps:
- Loaded and cleaned the dataset
- Separated the data into features (X) and labels (y)
- Split the data into training and testing sets
- Trained a Logistic Regression model
- Evaluated the model’s performance using accuracy, precision, recall, and F1-score

# Results
Logistic Regression Model:
- Accuracy: 0.99
- Precision:
    - For class 0 (healthy loan): 1.00
    - For class 1 (high-risk loan): 0.86
    
- Recall:
  - For class 0 (healthy loan): 0.99
  - For class 1 (high-risk loan): 0.94

- F1-Score:
  - For class 0 (healthy loan): 1.00
  - For class 1 (high-risk loan): 0.90

# Summary
The Logistic Regression model demonstrated strong performance in predicting loan status, achieving an overall accuracy of 99%. It is highly accurate in predicting healthy loans, with a precision and F1-score of 1.00, and it also performs well in predicting high-risk loans, with a recall score of 0.94 and an F1-score of 0.90.

## Recommendation
- The model is particularly well-suited for predicting healthy loans (0), as it correctly identifies almost all healthy loans and has a perfect precision score.
- For high-risk loans (1), the model still performs well, though there is a slightly lower precision (0.86), meaning some healthy loans might be falsely classified as high-risk. However, with a recall score of 0.94, the model is very effective at identifying actual high-risk loans, which is critical in a financial context where failing to identify a risky loan can have significant consequences.

Given its strong performance, particularly in identifying high-risk loans with a high recall score, I recommend using this model for the company’s loan risk predictions. The model’s ability to catch most high-risk loans while maintaining strong overall accuracy makes it a valuable tool for minimizing financial risks.
