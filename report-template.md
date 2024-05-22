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
    * Precision: Out of all the loans the model predicted "High risk" (1) , only 85% were high risk. 
    * Recall: Out of all the actual High risk , the model predicted this outcome correctly for 91% of those high risk loans.
    * Accuracy: the model has 99% acuraccy based on the TP(true positives) and TN (true negatives)out of all the total outcomes.
    * F1-score : The model has 0.88 score which is near 1.

## Summary

The logistic Regression model performs well in predicting the loan outcomes. 
* For healthy loans the prediction from the model are 100% correct with the test data. It only classifies 1% of healthy loans into high risk.
* For high risk loans (1) the 85% of model prediction matches with test data. This is happening because the dataset has very low of support for high risk loans (619) compared to the very high number of helathy loans(18765)

Keeping in mind that high risk loans are more harmful, the model needs to be better trained with more high risk loans to predict better.

