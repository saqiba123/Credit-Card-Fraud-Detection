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
![s2](https://user-images.githubusercontent.com/77055389/141067325-ea68bd43-cdb4-4c5f-85bb-9e3b5991f06e.PNG)

![s3](https://user-images.githubusercontent.com/77055389/141067351-a4279fe5-014a-4c55-90e0-b122b9117f55.PNG)

Plots
Class# 0=>not fraud
Class #1 => Fraud

-	Original dataset scatter plot.

![s4](https://user-images.githubusercontent.com/77055389/141067371-22dcd1c0-ebc0-45fd-b22d-0f4c1c931eee.PNG)

-	After Applying SMOTE Technique:

![s5](https://user-images.githubusercontent.com/77055389/141067400-94cfac51-66a8-4ac5-918f-2157ef0b5ca0.PNG)

-	Comparison Plot: 
![s6](https://user-images.githubusercontent.com/77055389/141067980-a3cc71e7-4329-4df7-8e7d-58f939059948.PNG)


-	Confusion Matrix heat Map

![s7](https://user-images.githubusercontent.com/77055389/141067428-86243fc9-c1d8-4f29-ab00-df93cd094484.PNG)

Conclusion:
We are getting fewer false positives, also we are catching a higher percentage of fraud cases. We are only using our test data to calculate the model results on. Few observations available to look at in the confusion matrix because we are using 30% of our dataset. Accuracy is about 99%, for not fraud transaction, to reduce the accuracy of not fraud transaction we simple use smote oversampling technique.by increasing the number of fraud transactions. We have reduced the accuracy to 98% as compared to previous model but the recall value of minority class has also improved to 92 %, this is a good model
