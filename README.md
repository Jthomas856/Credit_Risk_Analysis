# Credit_Risk_Analysis

## Overview
The purpose of this challenge is to apply machine learning to determine credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. We will employ different techniques to train and evaluate models with unbalanced classes. We will use a credit card dataset from LendingClub, we will oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we will use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we will compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally, we will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results
Six machine learning models were created to evaluate credit card risk. 

### Naive Random Oversampling
- The balanced accuracy score is 65%. The high-risk precision is low at 1%, the recall is 61%, which results in a F1 score of 2%.
 
<img width="478" alt="Screen Shot 2022-01-02 at 11 06 31 AM" src="https://user-images.githubusercontent.com/89098766/147881740-d11a31eb-ce76-4f01-9390-a2e456d917ae.png">
<img width="724" alt="Screen Shot 2022-01-02 at 11 06 45 AM" src="https://user-images.githubusercontent.com/89098766/147881747-5068d24c-f35c-4be0-a8c7-ba7d8830b310.png">

### SMOTE Oversampling
