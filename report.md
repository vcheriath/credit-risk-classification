# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

The purpose of this analysis is to identify when a loan is high-risk vs low-risk. To do so, a machine learning model was developed using logistic regression, trained on lending data that included factors such as loan size, interest rate, borrower income, debt/income ratio, and total debt. The data was split into a training set and a testing set so that the model could be evaluated on how well it predicted the risk-level of a loan.

A second model was created using random resampling, and this allowed us to train the model with a less imbalanced ratio of low-risk to high-risk loans. A more balanced ratio of low-risk to high-risk loans in the training data would theoretically make the model more effective at identifying high-risk loans.

## Results

* Machine Learning Model 1:
  * Model 1 had an accuracy of 0.99
  * The model had a precision of 1.00 for low-risk loans and a precision of 0.85 for high-risk loans, for a weighted average of 0.99
  * The recall score, the ability of the model to find positives, had a weighted average of 0.99 and was higher for the low-risk loans than for the high-risk loans



* Machine Learning Model 2:
  * Model 2 had an overall weighted accuracy of 0.99
  * the model had a precision of 1.00 for the low-risk loans and a precision of 0.84 for the high-risk loans, for a weighted average of 0.99
  * the recall score was 0.99 for both low-risk and high-risk loans

## Summary

* Model 1 had a slightly higher precision for high-risk loans, however Model 2 had a higher recall score. Therefore, Model 2 was determined to be the better performing model
* Given that it is more dangerous to underestimate the risk of a loan than it is to overestimate the risk, it is more important to predict when a loan will be high-risk. Therefore, an effective model should be stronger at identifying high-risk loans and not have many false negatives
