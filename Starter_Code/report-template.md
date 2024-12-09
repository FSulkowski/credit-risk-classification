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

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.



-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------


# Credit Risk Classification Report

## Overview of the Analysis

The purpose of this analysis was to evaluate a machine learning model's ability to predict the creditworthiness of borrowers using historical lending data. The dataset included financial information such as loan size, interest rates, and borrower income. The target variable was `loan_status`, where `0` indicated a healthy loan, and `1` indicated a high-risk loan.

The stages of the analysis included:
1. Splitting the data into training and testing sets.
2. Training a Logistic Regression model using the training data.
3. Evaluating the model's performance using metrics like accuracy, precision, and recall.

The logistic regression algorithm was chosen due to its suitability for binary classification problems.

## Results

### Logistic Regression Model:
- **Accuracy:** 99%
- **Precision:**
  - Healthy loans (0): 1.00
  - High-risk loans (1): 0.84
- **Recall:**
  - Healthy loans (0): 0.99
  - High-risk loans (1): 0.94

## Summary

The Logistic Regression model performs exceptionally well, achieving 99% overall accuracy. It predicts healthy loans with near-perfect precision and recall, making it highly reliable for identifying low-risk borrowers. For high-risk loans, the model demonstrates strong recall at 0.94, ensuring most high-risk loans are identified, though its precision of 0.84 indicates some false positives.

This model is recommended for use by the company as it provides a reliable tool for assessing credit risk. If the business prioritizes minimizing false positives for high-risk loans, additional tuning or alternative models may be considered to improve precision for high-risk predictions.
