# Module 12 Report Template

## Overview of the Analysis

The analysis in this report describes the machine learning techniques used to meet the challenge, the results obtained and the conclusions drawn, based on the findings. 

Purpose:
The purpose of the challenge was to evaluate machine learning models on loan risk. The starting point for the analysis was the resource dataset that contained historical lending activity from a peer to peer lending services company. The aim was to build a model that can identify the creditworthiness of borrowers. 

Methodology:
The process was set up by identifiying and installing the necessary components for the analysis. The data from the csv file was then read into a pandas dataframe for review. The data was then split into training and testing sets and then viewed to ensure the data was as expected. A critical part of the analysis was to be aware of the balance of the data numbers for the loan conditions. This was carried using the value_counts method. The data was then split into training and testing datasets to lay the foundations for the subsequent model application.
Logistic Regression was used to fit to the training data. The test data was then applied to the prediction model and then evaluated using accuracy score and confusion matrix along with a classification report. (Model 1)
Resampled Training data was then used using the RandomOverSampler module to allow for an analysis with an equal number of datapoints. (Model 2). Logistic Regression was again used with the "oversampled" data and an accuracy score, confusion matrix and classification report produced for comparison with the previous data. 


## Results

Using bulleted lists, describe the balanced accuracy scores and the precision and recall scores of all machine learning models.

* Machine Learning Model 1:

  * Description of Model 1 Accuracy, Precision, and Recall scores.
  *   Balanced Accuracy Score = 0.952
![Screenshot-Model1](https://user-images.githubusercontent.com/113118793/225910415-22ec9e87-0dc4-4468-8a35-9d23c187503e.jpg)


* Machine Learning Model 2:
  * Description of Model 2 Accuracy, Precision, and Recall scores.
  *  Balanced Accuracy Score = 0.993
![Screenshot-Model2](https://user-images.githubusercontent.com/113118793/225910473-769430cb-400f-46e2-b4cb-62a9082500ae.jpg)


 * The balanced accuracy score is improved using the resampled (oversampling) process from 0.95 to 0.99.
 * The revised analysis using the oversampling technique has given a greater balanced performance for the loan conditions. For the high-risk loans, with only a very minor reduction in precision from 0.85 to 0.84, the recall and f1-score are improved 0.91 to 0.99 and 0.88 to 0.91 respectively.


## Summary

As can be seen from the resuilts above, the Machine Learning Model 2 gives the better perfromance of the two investigated. The summary statistics produced in the study describe this, with improved values nearer to one obtained with the model2 application. The performance of any model is required to predict more accurately the high-risk loans as it is these that require further management (i.e. loan refused or restrucutred). Model 2 shows the benefits of having a more balanced number of data points for the 2 conditions rather than the biased number in Model 1.
Therefore Model 2 would be the recommended Model to the lending services company.  

