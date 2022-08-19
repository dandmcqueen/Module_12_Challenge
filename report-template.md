# Module 12 Report

## Overview of the Analysis

<br/>

In this analysis, a logistic regression model is built to determine whether or not credit borrowers are 
high risk.  2 models are compared, one that uses the original date, and a second that is adjusted for imbalancing.

The data set comes from a peer-to-peer lending service. The analysis attempts to predict the loan_status
as either a 0(for healthy loans) or a 1(high-risk loans).

The standard model, fit , predict, process was used in building the models. Train_test_split is used to seperate 
the training data from the testing data. Both models are fit with LogisticRegression, with the second model resampled
with RandomOverSampler.


---

<br/>

## Results


* Machine Learning Model 1:

  * Balanced accuracy is 95%
  * Precision is 99% for healthy loans and 85% for high-risk loans
  * Recall is 99% for healthy loans and 91% for high-risk loans

<br/>

* Machine Learning Model 2 Resampled:
  * Balanced accuracy is 99%
  * Precision is 100% (0.999) for healthy loans and 84% for high-risk loans
  * Recall is 99% for both healthy and high-risk loans

---

<br/>

## Summary

Both models have a high accuracy showing a strong ability to predict healthy loans.  Each have a similar precision for high-risk loans, however
the recall is almost 10% higher for high-risk in the resampled data, showing a greater ability to predict high-risk loans.  This improvement puts 
the resampled model over the original data model as predicting high-risk loans is the overall goal of these two models.

