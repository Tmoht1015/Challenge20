# Module 12 Report 

## Overview of the Analysis

The goal of this study is to see how well two computer models can predict whether a loan is risky or not by looking at financial information. I used data about loan size, interest rates, borrower income, and other factors in order to determine if a loan is safe (0) or risky (1).

To begin, our data is divided into two parts for training and testing.
I made one model with the original data and checked how well it worked, measuring the model's accuracy, precision, and recall.
To handle an imbalance in the data, more examples were added using a technique called RandomOverSampler.
Then, we created another model with the new, balanced data and checked how well it worked using the same measurements above.

+ two methods in this study: LogisticRegression and RandomOverSampler.

## Results

Machine Learning Model 1 with Original Data:

+ Accuracy: The model is very accurate, correctly classifying 99% of cases.
+ Precision for healthy loans (0): Excellent at identifying true positives with very few mistakes.
+ Precision for high-risk loans (1): Moderately effective in spotting high-risk loans with some errors.
+ Recall for healthy loans (0): Correctly identifies nearly all healthy loans with very few misses.
+ Recall for high-risk loans (1): Effective at identifying high-risk loans with some misses.

Machine Learning Model 2 with Resampled Data:

+ Accuracy: The model is also very accurate, correctly classifying 99% of cases.
+ Precision for healthy loans (0): Excellent at identifying true positives with very few mistakes.
+ Precision for high-risk loans (1): Very effective in spotting high-risk loans with very few mistakes.
+ Recall for healthy loans (0): Correctly identifies nearly all healthy loans with very few misses.
+ Recall for high-risk loans (1): Very effective at identifying high-risk loans with very few misses.

## Summary

Model 2, the logistic regression model trained with the resampled data, outperforms Model 1 trained with the original data. It is particularly better at predicting high-risk loans, with higher precision and recall scores. This is important for reducing financial risks for the lending company.

I recommend using Model 2 for credit risk analysis! It significantly improves the prediction of high-risk loans compared to model 1. This choice will enable the company to assess loan applications effectively and make informed decisions when approving or rejecting loans, reducing credit risk.