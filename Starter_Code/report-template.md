# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

The purpose for this analysis was to create a supervised learning model to accurately predict healthy loans vs high-risk loans. The model we used to try and achieve this was a logistic regression model. The information that was given to us to create this model was part of a CSV file that we read into a dataframe. This information included loan size, interest rate, borrower income, debt to incone, number of accounts, derogatory remarks, and total debt. We needed to predict the loan status which was based on binary classification, 0 being a healthy loan while 1 signified a high-risk loan, hence the use of a logistic regression model.

As part of this analysis, we had to split the data gathered into test and training sets using the train_test_split module. Using LogisticRegression which we imported from SKLearn, we fit the training data to our linear regression model and made predictions using the test data and we evaluated its predictions based on a confusion matrix and classification report.

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model (Logistic Regression Model):
    Accuracy - 0.99, meaning it correction classified 99% of all loans

    Precision: 
    Healthy Loan (0) - 1.00
    High-Risk Loan (1) - 0.84

    Recall:
    Healthy Loan (0) - 0.99
    High-Risk Loan (1) - 0.94

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.

The logistic regression model did a near-perfect job classifying healthy loans, predicting them at a rate of 1.00 while predicting the high-risk loans at a rate of 0.84 which is still very good. We know that this performance is very good because the accuracy we get from the classification report is 0.99 or 99%. It is more important to predict the 1s (high-risk loans) since those types of loans could be more detrimental to lenders. Flagging those that are high-risk rather than thos who are healthy could prove to be more beneficial than flagging those that are healthy vs high-risk.
