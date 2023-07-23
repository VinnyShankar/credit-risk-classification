# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* This data is about loans. Each row represents one loan, and the columns represent the metadata for that loan (things like loan size, interest rate, borrower's income, etc). Each loan has been labeled as "healthy" or "high-risk."
* There are two main purposes for this analysis. The first is to test how well a supervised learning model can predict the correct label for a loans ("healthy" or "high risk"). The second purpose is to see if the model's performance improves when random oversampling is introduced. The main methods used were Logistic Regression and RandomOversampling.
* The stages of machine learning in this study are:
  - Separate the labels column from the rest of the data
  - Separate the labels and data into training and testing sets
  - Fit the training data to a Logistic Regression model
  - Predict the labels for the testing data
  - Assess the model's performance based on the balanced accuracy score, the confusion matrix, and the classification report
  - Repeat the previous steps after using Random Oversampling on the training data

## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.



* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
