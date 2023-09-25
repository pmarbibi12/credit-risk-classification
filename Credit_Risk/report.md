# Module 12 Report

## Overview of the Analysis

* This analysis aims to develop an algorithm for accurately assessing the health or risk associated with loans. By utilizing logistic regression and supervised machine learning techniques, I successfully created a model capable of determining whether a loan is healthy or high-risk with an impressive 99% accuracy rate. The model achieves this accuracy by analyzing key factors such as loan size, interest rate, borrower income, debt-to-income ratio, number of accounts, derogatory marks, and the total debt for each loan. Additionally, I explored the use of oversampled data with another model, which also achieved a commendable 99% accuracy rate.


## Results

* Machine Learning Model 1:
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  - Accuracy: 0.9918489475856377
  - Precision `0`:  0.99
  - Recall `0`:     1.00
  - Precision `1`:  0.91
  - Recall `1`:     0.85

* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  - Accuracy: 0.9938093272802311
  - Precision `0`:  0.99
  - Recall `0`:     1.00
  - Precision `1`:  0.99
  - Recall `1`:     0.84

## Summary

Which one seems to perform best? How do you know it performs best?
- The second model appears to outperform the first one. This conclusion is based on the second model achieving a higher precision score in assessing loan high-risk status.

Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
- Indeed, performance does hinge on the problem we are tackling. In this case, it holds greater significance to identify high-risk accounts than to determine the healthiness of a loan. A healthy loan typically requires no intervention, whereas detecting a high-risk loan can be vital for taking appropriate actions.

If you do not recommend any of the models, please justify your reasoning.
* In this case, I would recommend employing random oversampling. Random oversampling is designed to address class distribution imbalances. By bringing the samples closer to a balanced state, it enhances predictive performance by mitigating class bias. It's important to note, however, that there is a risk of overfitting when using oversampling. Therefore, it's advisable to apply oversampling primarily to datasets where the class imbalance is not excessively high.
