# Predicting Loan Risk with Machine Learning

## Overview

In this analyis, our goal was to create a machine learning model to predict the creditworthiness of borrowers for a peer-to-peer lending services company. 

* In this dataset, a value of 0 means the loan is healthy, and a value of 1 means the loan is at high-risk of defaulting.
* The original data set included 77,536 entries in the following proportions:
  * 75,036 healthy loans
  * 2,500 high-risk loans
* We looked at a variety of features in the dataset, including loan size, interest rate, borrower income, debt to income ratio, number of accounts, and total debt.
* We created this model using a `LogisticRegression` method.
* To create the model, we took the following steps:
  * Import the original data CSV using Pandas.
  * Separate the labels, or y, from the features, or x.
  * Split the data into training and testing datasets using `train_test_split`.
  * Create the `LogisticRegression` model using the training datasets.
  * Predict the results of the test dataset and compare to the y_test data
  * Evaluate the model's performance

## Results

The machine learning model we created using a logistic regression yielded the following results:
* Balanced Accuracy Score = 0.952
* Confusion Matrix:
  * 18,663 true negatives
  * 563 true positives
  * 102 false positives
  * 56 false negatives
* Negative Results:
  * Precision = 1.00
  * Recall = 0.99
* Positive Results:
  * Precision = 0.85
  * Recall = 0.91


## Summary

Overall, this model does a decent job predicting both healthy and high-risk loans. It is very good a predicting healthy loans, with a precision of 100% and a recall of 99%. It is a little less successful at predicting high-risk loans, with a precision of 85% and a recall of 91%, but these are still acceptable results in my opinion. The balanced accuracy score of the model is approximately 95%, which supports that the model is doing a good job predicting results of loans.
