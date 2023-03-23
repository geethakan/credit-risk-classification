<div><img align=left width=200px height=120px src="https://github.com/geethakan/credit-risk-classification/blob/main/Credit_Risk/Resources/credit-risk-model.png">
  
# Supervised Learning - Logistic Regression Model
  
In this exercise, dataset of historical lending activity from a peer-to-peer lending services company is used to build a model that can identify the creditworthiness of borrowers.</div>

### Introduction
Supervised learning, also known as supervised machine learning, is a subcategory of machine learning and artificial intelligence. A computer algorithm is trained on input data that has been labeled for a particular output. The model is trained until it can detect the underlying patterns and relationships between the input data and the output labels, enabling it to yield accurate labeling results when presented with never-before-seen data. Supervised learning is good at classification and regression problems. 

 - A classification algorithm aims to sort inputs into a given number of categories or classes, based on the labeled data it was trained on. Classification algorithms can be used for binary classifications for eg. categorizing customer feedback as positive or negative, categorizing emails into spam or non-spam etc. 
 - Regression analysis is a powerful statistical method that allows one to examine the relationship between two or more variables of interest. Regression can be linear or logistic regression.
    - Linear Regression is used to handle regression problems and provides a continuous output.
    - Logistic regression is used to handle the classification problems and provides discreet output.  
 
 
 ### Steps involved in this Logistic Regression modelling
  #### Purpose
  Create a logistic regression model and train using about 75% of the dataset. Use 25% of data to test the results. Run classification report to analyze results and conclude on the strength of the model for predicting new data.
  
  #### Dataset
  Following were the fields used from csv of lending information
   - Income of borrower
   - Loan Amount 
   - Loan rate 
   - Total debt 
   - Income to debt ratio
   - Number of accounts
   - Count of derogatory marks
   - Loan Status - 0 = healthy and 1 = high-risk
   
   Total records in dataset: 77536
   - Healthy loans: 75036   High-risk: 2500
   
   Training counts:
   - Healthy: 56277         High-risk: 1875
   
   Testing counts:
   - Healthy: 18759        High-risk: 625
   
  #### Machine Learning
  - csv loaded into pandas dataframe
  - data is separated into features (X) and labels (y)
  - Sklearn train_test_split function used to split dataset into training data and test data (default split of 75% for training and 25% for testing. stratify=y specified to maintain the ratio of healthy and unhealthy loans in the train and test splits)
  - Instantiate LogisticRegression model and fit it with training data.
  - Use test feature data and get predictions of the labels.
  - Evaluate the performance using accuracy score, confusion matrix and classification report.
  - Image of classification report shown below:
  <div><img align=left width=600px height=300px src="https://github.com/geethakan/credit-risk-classification/blob/main/Credit_Risk/Resources/classification_report.png"></div>
  
 #### Summary
  

  
