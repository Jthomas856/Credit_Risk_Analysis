# Credit_Risk_Analysis

## Overview
The purpose of this challenge is to apply machine learning to determine credit card risk. Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. We will employ different techniques to train and evaluate models with unbalanced classes. We will use a credit card dataset from LendingClub, we will oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we will use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we will compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Finally, we will evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Results
Six machine learning models were created to evaluate credit card risk. 

### Naive Random Oversampling
- The balanced accuracy score is 65%. 
- TThe high-risk precision is low (1%) and the low-risk precision is high (100%).
- The recall is 72% for high-risk and 59% for low-risk.
- The high-risk F1 score is 2%.
 ![Screen Shot 2022-01-02 at 12 50 13 PM](https://user-images.githubusercontent.com/89098766/147884657-75bb98d8-f3cb-4410-b976-6d951b81b3ad.png)


### SMOTE Oversampling
- The balanced accuracy score is 66%. 
- The high-risk precision is low (1%) and the low-risk precision is high (100%). 
- The recall is 63% for high-risk and 69% for low-risk.
- The high-risk F1 score is 2%.
![Screen Shot 2022-01-02 at 12 51 58 PM](https://user-images.githubusercontent.com/89098766/147884743-db01ad7c-1d9c-40f1-b4bb-d586a1b1e5ea.png)


### Undersampling
- The balanced accuracy score is 54%. 
- The high-risk precision is low (1%) and the low-risk precision is high (100%). 
- The recall is 69% for high-risk and 40% for low-risk.
- The high-risk F1 score is 1%.
![Screen Shot 2022-01-02 at 12 53 52 PM](https://user-images.githubusercontent.com/89098766/147884818-8d91f392-fcb2-4a9c-8ebd-986363ab84a7.png)


### SMOTEENN Combination Sampling



### Balanced Random Forest Classifier
- The balanced accuracy score is 79%. 
- The high-risk precision is 4% and the low-risk precision is 100%. 
- The recall is 67% for high-risk and 91% for low-risk. 
- The high-risk F1 score is 7%.
![Screen Shot 2022-01-02 at 12 58 19 PM](https://user-images.githubusercontent.com/89098766/147884934-b0eab4a0-5cfb-4186-a147-a20289e35d5d.png)


### Easy Ensemble AdaBoost Classifier
- The balanced accuracy score is 93%. 
- The high-risk precision is 7% for high-risk and 100% for low-risk. 
- The recall is 91% for high-risk and 94% for low-risk. 
- The high-risk F1 score is 14%.
![Screen Shot 2022-01-02 at 1 00 03 PM](https://user-images.githubusercontent.com/89098766/147884975-b8cc531f-fbf5-432a-8305-2efdfb10ed6e.png)


## Summary

The results for all 6 machine learning models varied slightly. All of the models yielded low precision scores for predicting high-risk, but scored high precision in predicting low-risk. The Undersampling model had the lowest balanced accuracy score at 54%, and the Easy Ensemble AdaBooster Classifier had the highest at 93%. The classifier models showed improvement in the overall prediction results, especially with the recall predictions meaning they were more sensitive at predicting high-risk credit which is useful in our case of analyzing credit risk. Overall though there is not one perfect model, I would recommend the Easy Ensemble AdaBoost Classifer model for its high balanced accuracy score, decently balanced recall score, and the highest precision of all the models at predicting high risk.
