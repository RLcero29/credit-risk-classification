The purpose for this analysis was to create a supervised learning model to accurately predict healthy loans vs high-risk loans. The model we used to try and achieve this was a logistic regression model. The information that was given to us to create this model was part of a CSV file that we read into a dataframe. This information included loan size, interest rate, borrower income, debt to incone, number of accounts, derogatory remarks, and total debt. We needed to predict the loan status which was based on binary classification, 0 being a healthy loan while 1 signified a high-risk loan, hence the use of a logistic regression model.

As part of this analysis, we had to split the data gathered into test and training sets using the train_test_split module. Using LogisticRegression which we imported from SKLearn, we fit the training data to our linear regression model and made predictions using the test data and we evaluated its predictions based on a confusion matrix and classification report.
<br>
<br>
Machine Learning Model (Logistic Regression Model): Accuracy - 0.99, meaning it correction classified 99% of all loans

Precision: Healthy Loan (0) - 1.00 High-Risk Loan (1) - 0.84

Recall: Healthy Loan (0) - 0.99 High-Risk Loan (1) - 0.94
