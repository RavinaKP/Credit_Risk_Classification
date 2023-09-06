# Credit_Risk_Classification
## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

## Results
* Original Logistic Regression Model 1:
  * Accuracy Score: 99%
  * Precision Score for Class 0 (Healthy loans): 100%
  * Precision Score for Class 1 (High-risk loans): 85%
  * Recall Score for Class 0: 99%
  * Recall Score for Class 1: 90%
    * Confusion matrix details of test data:
      * True Positives (TP): 18,695 cases of healthy loans were correctly identified
      * True Negatives (TN): 533 cases of high-risk loans were correctly identified
      * False Positives (FP): 71 cases of high-risk loans were incorrectly classified as healthy loans
      * False Negatives (FN): 85 cases of healthy loans were incorrectly classified as high-risk loans 

* Logistic Regression Model with Resampled Training Data Model 2:
  * Accuracy Score: 99%
  * Precision Score for Class 0 (Healthy loans): 100%
  * Precision Score for Class 1 (High-risk loans): 86%
  * Recall Score for Class 0: 99%
  * Recall Score for Class 1: 100%
    * Confusion matrix details:
      * True Positives (TP): 18,682 cases of healthy loans were correctly identified
      * True Negatives (TN): 601 cases of high-risk loans were correctly identified
      * False Positives (FP): 98 cases of high-risk loans were incorrectly classified as healthy loans
      * False Negatives (FN): 03 cases of healthy loans were incorrectly classified as high-risk loans 

## Summary

* Summary and Recommendations:

    * The original logistic regression model achieved impressive accuracy, precision, and recall scores for classifying healthy loans         (Class 0), with an accuracy of 99%, precision of 100%, and recall of 99%. However, its performance for identifying high-risk loans (Class 1) was less satisfactory, with a precision of 85% and a recall of 90%. This indicates that the model is highly precise in  predicting healthy loans but less reliable in flagging high-risk loans. In the context of a financial institution, the primary          concern is correctly identifying high-risk loans to mitigate potential losses.

    * To address this issue, a logistic regression model with resampled training data was employed. This balanced data approach improved the model's performance significantly in identifying high-risk loans. The accuracy remained at 99%, and the precision for high-risk loans increased to 86%, while recall reached 100%. This means that the model is highly precise and accurate in identifying both healthy and high-risk loans after the data balancing.

* Recommendation:

Based on the analysis results, it is recommended to use the logistic regression model with resampled training data for identifying the creditworthiness of borrowers. This model offers an excellent balance between precision and recall for both healthy and high-risk loans, making it a valuable tool for a financial institution's lending decision process. The balanced data approach ensures that the model is equally effective in identifying both types of loans, reducing the risk of approving high-risk loans and minimizing potential losses for the company.
