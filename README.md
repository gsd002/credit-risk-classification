# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of this analysis is to develop a machine learning model that can accurately predict the risk associated with loan applications. By using logistic regression, the aim is to classify loans into healthy (0) and high-risk (1) categories based on various financial indicators.

* Explain what financial information the data was on, and what you needed to predict.
The data was on historical lending activity from a peer-to-peer lending services company. It consists of features such as loan_size, interest_rate, borrower_income, debt_to_income, num_of_accounts, derogatory_marks, total_debt, and the target variable loan_status. The 'loan_status' column, indicates whether a loan is healthy (0) or has a high risk of defaulting (1). We need to build a model that can identify the creditworthiness of borrowers.

* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
The target variable 'loan_status' shows that there are 75,036 loans that were healthy (0) and 2,500 loans that were high-risk (1). The data has been successfully split into training and testing sets. We have 58,152 samples in the training set and 19,384 samples in the testing set, with each sample containing 7 features.

* Describe the stages of the machine learning process you went through as part of this analysis.
  1) Understanding the problem
  2) Data preparation
  3) Spliting the data into training and testing sets
  4) Model selection and training
  5) Model evaluation
  7) Interpretation and reporting

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
    Accuracy Score: The model achieved an overall accuracy of 99%.
    Precision Score:
      Healthy loans (0): 1.00
      High-risk loans (1): 0.84
    Recall Score:
      Healthy loans (0): 0.99
      High-risk loans (1): 0.94


## Summary

Summarise the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
The logistic regression model demonstrates exceptional performance in identifying healthy loans with perfect precision and recall scores. It also showes a strong capability in detecting high-risk loans, though with slightly lower precision and recall. 
This indicates that while the model is highly reliable in classifying loans, there's a minor chance of misclassifying high-risk loans as healthy. 
Given the model's high overall accuracy, it is recommended for use in evaluating loan applications to identify potential risks. 
However, for critical financial decisions, additional checks or a combination of models could be considered to further minimize the risk of misclassification.

