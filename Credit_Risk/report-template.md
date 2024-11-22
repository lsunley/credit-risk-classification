# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
* Explain what financial information the data was on, and what you needed to predict.
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
* Describe the stages of the machine learning process you went through as part of this analysis.
* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any other algorithms).

## Results

Using bulleted lists, describe the accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:
    * Description of Model 1 Accuracy, Precision, and Recall scores.

## Summary
Summarize the results of the machine learning models, and include a recommendation on the model to use, if any.

## Which Model Performs Best?
* The Logistic Regression model performs well overall and is particularly effective at identifying the majority class (0).
* It demonstrates strong performance for the minority class (1), especially with high recall (94%), which is critical in certain contexts.

## Does Performance Depend on the Problem?
* If predicting high-risk loans (1) is more critical:
The recall for 1 is 94%, meaning the model correctly identifies most high-risk loans. This is ideal if the goal is to minimize the risk of missing true high-risk loans, even if it means a few healthy loans are flagged incorrectly.
* If predicting healthy loans (0) is more critical:
The model’s perfect precision (1.00) and high recall (0.99) for 0 ensure minimal misclassification of healthy loans.

The performance depends on the cost or risk associated with misclassifying either category:
* Missing a high-risk loan (1) could lead to financial loss or risk exposure.
* Misclassifying a healthy loan (0) as high-risk may result in unnecessary investigation or customer dissatisfaction.

## Recommendation:
Use the Logistic Regression model.
* It demonstrates strong overall performance and balances the trade-off between precision and recall for both labels.
* The high recall for high-risk loans (1) ensures critical cases are identified, while the near-perfect performance for healthy loans (0) minimizes false positives.