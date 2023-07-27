# Machine Learning to Predict Credit Risk

## Credits
- Author: Vinny Shankar
- Acknowledgements:
    - Study Groups: worked together with several students to understand the assignment
    - Students: [Hany Dief](https://github.com/hanydief), [Jed Miller](https://github.com/Jed-Miller), [Jésus Jímenez](https://github.com/JesusJimenez3318), [Shridhar Kamat](https://github.com/shriparna), [Borna Karimi](https://github.com/karimiborna)
    - Program: University of California Berkeley Data Analytics Bootcamp
    - Starter Code: The Module Challenge provided starter code that guided the process
    - Instructor: Ahmad Sweed

## Overview

* The dataset in this study pertains to loans from a peer-to-peer lending company. Each row represents one loan, and the columns represent the metadata for that loan (things like loan size, interest rate, borrower's income, etc). Each loan has been pre-labeled as "healthy" or "high-risk."
* There are two main purposes for this analysis. The first is to test how well a `KMeans` supervised learning model can predict the correct label for a loan. The second is to see if the model's performance improves when random oversampling is introduced. The main methods used are Logistic Regression and Random Oversampling.
* The machine learning steps are as follows:
  - Separate the labels column from the rest of the data (features)
  - Separate the labels and features into training and testing sets
  - Fit the training data to a Logistic Regression model
  - Predict the labels for the testing data
  - Assess the model's performance based on the balanced accuracy score, the confusion matrix, and the classification report
  - Repeat the Logistic Regression, Prediction, and Assessment after using Random Oversampling on the training data

## Results

* Machine Learning Model 1:
  * Balanced Accuracy Score: 0.95
  * Precision (Healthy Loans): 1.00
  * Recall (Healthy Loans): 0.99
  * Precision (High Risk Loans): 0.85
  * Recall (High Risk Loans): 0.91
  * True Positives: 18663
  * False Positives: 102
  * True Negatives: 563
  * False Negatives: 56
* Machine Learning Model 2:
  * Balanced Accuracy Score: 0.99
  * Precision (Healthy Loans): 1.00
  * Recall (Healthy Loans): 0.99
  * Precision (High Risk Loans): 0.84
  * Recall (High Risk Loans): 0.99
  * True Positives: 18649
  * False Positives: 116
  * True Negatives: 615
  * False Negatives: 4

## Summary

* `Machine Learning Model 2` (Random Oversampling) seems to perform the best because it has a higher balanced accuracy score, almost no Type 2 errors (False Negatives), and higher recall for high-risk loans.
* Performance depends on the data being used. However, the interpretation of the performance changes depending on the context.
* For example, if a company wants to completely avoid lending to high-risk borrowers, that company will place more importance on predicting the `1`'s with higher precision (they will have less tolerance for mislabeling the `1`'s).
* In another example, if a company is willing to lend to high-risk borrowers (while collecting a higher interest rate), that company will place less importance on predicting the `1`'s (they will have higher tolerance for mislabeling the `1`'s).