# Credit-Card-Fraud-Detection


DATASET:

This project uses the Credit Card Fraud Detection dataset from Kaggle.
European Dataset. The datasets contain transactions made by credit cards in September 2013 by European cardholders. This dataset presents transactions that occurred in two days, where we have 492 frauds out of 284,807 transactions. The dataset is highly unbalanced, the positive class (frauds) account for 0.172% of all transactions.

Features V1, V2, … V28 are the principal components obtained with PCA, the only features which have not been transformed with PCA are 'Time' and 'Amount'. Feature 'Time' contains the seconds elapsed between each transaction and the first transaction in the dataset. The feature 'Amount' is the transaction Amount, this feature can be used for example-dependant cost-senstive learning. Feature 'Class' is the response variable and it takes value 1 in case of fraud and 0 otherwise.

![s1](https://user-images.githubusercontent.com/77055389/141066963-157fb724-25f1-4bdf-b74f-cc89a5731a4a.PNG)

Methodology:

Step1: Import the Libraries
Step2: Load the dataset
Step3: Apply data preprocessing on the loaded dataset.
Step4: Define the resampling method using SMOTE technique
Step5: plot the original data and also plot the resampled data.
Step6: Create the training and testing sets 70% for training and 30% for Testing.
Step5: Fit a logistic regression model to our data
Step6: Show the classification report and confusion matrix
Step7: Define the pipeline, tell it to combine SMOTE with the Logistic Regression model.






Result:

 

 

 

Plots
Class# 0=>not fraud
Class #1 => Fraud




-	Original dataset scatter plot.


-	After Applying SMOTE Technique:






-	Comparison Plot: 

-	Confusion Matrix heat Map

 
Conclusion:
We are getting fewer false positives, also we are catching a higher percentage of fraud cases. We are only using our test data to calculate the model results on. Few observations available to look at in the confusion matrix because we are using 30% of our dataset. Accuracy is about 99%, for not fraud transaction, to reduce the accuracy of not fraud transaction we simple use smote oversampling technique.by increasing the number of fraud transactions. We have reduced the accuracy to 98% as compared to previous model but the recall value of minority class has also improved to 92 %, this is a good model
