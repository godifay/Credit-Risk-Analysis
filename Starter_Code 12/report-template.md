# Module 12 Report Template

## Overview of the Analysis

In this section, describe the analysis you completed for the machine learning models used in this Challenge. This might include:

* Explain the purpose of the analysis.
The purpose of the report is to analyse a credit risk based on the the dataset provided by appliying machine learning model. 
* Explain what financial information the data was on, and what you needed to predict.
The financial information is based on the dataset of historicaly lending activities and to predict the creditworthiness of borrowers. 
* Provide basic information about the variables you were trying to predict (e.g., `value_counts`).
From the basic information provided , the value count shows there are healthy loans(0) and high-risky loans(1) , the value count yeilds 75036 and 2500 respcetivly , which also tells imbalanced class to predict i.e the existing classes in a dataset aren't equally represented.
* Describe the stages of the machine learning process you went through as part of this analysis.
Classify the variable to features and predictive values i.e Separate the data into labels and features, i.e the loan status. 
Determine the value counts to see how reprsetative the classes are .
Split the Data into Training and Testing Sets
Create a Logistic Regression Model with the Original Data
Predict a Logistic Regression Model with Resampled Training Data
Interpret the accuracy , precision and recall of the models being used .

* Briefly touch on any methods you used (e.g., `LogisticRegression`, or any resampling method).

Logistic regression method is used to fit a regression model  to predict the classes , healthy loan and high risk loan and resampling method i.e oversampling  used to artificially balance the classes that the model gets during training, in this analysis the  resmapling method helps the model avoid hyperfocusing on the larger class ( healthy loan )and can improve the predictions for the smaller class( high-risk loan)
## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1: linear regression .
  * Description of Model 1 Accuracy, Precision, and Recall scores.
  
  Accuracy :94.8%
  Precision : 100% for the healthy loan and 85% for the risky loan
  Recall :99% for the healthy loan and 90 % for the risky loan
  

* Machine Learning Model 2: Linear regression and oversmapling 
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  Accuracy : 99.36 % for resmapled method, oversampling .
  Precision : 100% for the healthy loan and 84% for the risky loan 
  Recall : 99 % for both the healthy loan and the risk loan .

N.B recall measures the percentage of healthy laons and risky loan  that the model correctly classified as healthy or risky one ( True positive and True negative)
## Summary

Summarize the results of the machine learning models, and include a recommendation on the model to use, if any. For example:
* Which one seems to perform best? How do you know it performs best?
Given the orginal data, the precision for minority class( the high risk loan), i.e when its pridicted how often its corect is a little higher than the resmapled data, which is 85% and 84% respcetively . Howerver, the accuracy report is on original data is lower than the resampled data,  , jumps from 94.8% to 99.36%. Similarily , the recall on orginal data is 90% but on the resampled model has shown a 9% improvement a great improvement in detecting the true positive and true negative. 
* Does performance depend on the problem we are trying to solve? (For example, is it more important to predict the `1`'s, or predict the `0`'s? )
The performace  on accuracy  and recall on the resampled model has shown improvements , eventhough its based on the need of the organization , if for example want to give more weight on the status of the risky loan, the resampled model recommended as its in better position in identfying  the risky loans .




