# Overview of the Analysis

In this analysis a machine learning model is created to evaluate the credit worthiness of borrowers. A dataset of historical lending activity from a peer-to-peer lending services company is used to build the model.

## Data Info:

*  The dataset included historical lending activity data, information is based on borrower's income, loan size, interest rate and debit to income ration. With the final outcome on loan status, A value of 0 in the loan_status column means that the loan is healthy. A value of 1 means that the loan has a high risk of defaulting.

* The dataset has a size of 77536. 

## Machine Learning 

The machine learning model is created to predict the loan status based on different features in the data.

y variable: This the labels. It is the 'loan_status' column, where 0 represents healthy loans, and 1 represents high-risk loans.
X variable: These are the features. It is a dataframe consisting of everything except the label. It has 7 columns.

## ML stages:

   * Preprocess: Reading the data from CSV, defining X and y variables and splitting it into subsets for training and testing the model.
   * ML model: Logistic Regression Modeling is used here as the outcomes are binary from data.
   * Train : A large subset of the labeled data is used to teach the model to recognize classification patterns.
   * Predict: Finally, the model is used to predict labels for unclassified data(test data).

## Results

* Logistic regression model:
    * Accuracy: 

## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:

* Which one seems to perform best? How do you know it performs best?
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )

If you do not recommend any of the models, please justify your reasoning.
