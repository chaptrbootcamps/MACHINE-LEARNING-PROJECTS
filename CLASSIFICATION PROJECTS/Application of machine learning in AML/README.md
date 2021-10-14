# Fraud detection using credit cards transaction dataset
The Institute of International Finance and Deloitte LLP highlights that: There is growing consensus that the current global framework for fighting financial crime is not as effective as it could be and that more needs to be done at the international, regional and national levels to help identify and stem the flow of illicit finance – an activity which supports some of the worst problems confronting society today, including terrorism, sexual exploitation, modern slavery, wildlife poaching and drug smuggling.

Whilst these problems in themselves are pressing and need a multifacted approach for resolution, financial institutions are facing even greater pressure to modernize and make more robust their AML functions for various risk management objectives. 

ML has transformed the KYC processess and transaction monitoring functions. To further improve the customer onboarding there is need to contsantly improve the customer due dilligence processs (CDD) through recalllibration of these models and effective model governance. 

![](https://th.bing.com/th/id/OIP.RzTZtIe43i0FD4frdhe0SAHaE9?w=298&h=200&c=7&r=0&o=5&pid=1.7)

In this project you will use dataset found in [Kaggle](https://www.kaggle.com/mlg-ulb/creditcardfraud) containing transcation made in Sept 2013 by European card holders which occured in the course of 2 days. 
This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.
It contains only numerical input variables which are the result of a PCA transformation. Unfortunately, due to confidentiality issues more background cannot be provided about the features. 

Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-sensitive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

Given the class imbalance ratio, we recommend measuring the accuracy using the Area Under the Precision-Recall Curve (AUPRC). Confusion matrix accuracy is not meaningful for unbalanced classification.

In this project you will  use and learn about the various oversampling and undersampling techniques are why these are useful in varous classfication problems. 

You will also get to lean why different [classification](https://www.kaggle.com/kaanboke/the-most-common-evaluation-metrics-a-gentle-intro) metrics are used in the case of unbalanced data. 
 
You will find the following information useful in understanding the nature of the presented features. 
- Every customer has a unique profile. That is their geoographical location, spending frequency and amounts. 
- The transactions happen in different terminals, merchants, or ATMs which are based in certain geographical locations. 
- There is an association of customers to terminals in the sense that customers are likely to make transactions in terminals geographically close to their locations. 
