# Credit-Risk-Analysis-

## Overview 

Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. In this project, we will use imbalanced-learn and scikit-learn libraries to build and evaluate models using resampling. Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, we'll oversample the data using the RandomOverSampler and SMOTE algorithms, and undersample the data using the ClusterCentroids algorithm. Then, we’ll use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. Next, we’ll compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. 

## Results

- Naive Random Oversampling results: 
 
Balanced accuracy test is 67%. The precision for the high risk is at 1%, and the recall is 60%.
 
![image](https://user-images.githubusercontent.com/88631769/147399436-374dd258-943b-4f67-b8c2-b1d699dce498.png)

- SMOTE oversampling results: 

The accuracy score is 65%. The precision for the high risk is at 1%, and total recall is 66%. 

![image](https://user-images.githubusercontent.com/88631769/147399557-03be95d5-e343-4fd5-ba34-5d6c83745850.png)

- Undersampling results: 

The accuracy score is at 65%. The precision is 99%, and the total recall is 44%.
![image](https://user-images.githubusercontent.com/88631769/147399709-b457e7cf-2e56-4b3e-bda6-9ee5223f049b.png)

- Combination(over and undersampling) results:

The accuracy score is 51%. The precision is 99%, and the total recall is 57%. 

![image](https://user-images.githubusercontent.com/88631769/147399834-0171567e-8600-46a7-b447-1df272d3ab04.png)


- Balanced Random Forest Classifier results: 

The accuracy score is 78%. The precision for the high risk is 99%, and the recall is 91%. 

![image](https://user-images.githubusercontent.com/88631769/147399892-4d66c161-2a18-470d-bff1-cf544dfa03fd.png)

- Easy Ensemble AdaBoost Classifier results:
 
 AttributeError: 'EasyEnsembleClassifier' object has no attribute 'estimators_'. Unable to get the result. 
 
 
## Summary 

In the first four models, the accuracy score is not as high as the ensemble classifer and the recall in the oversampling/undersampling/mixed models is relatively low. To acquire a balance of recall and precision, we should use ensemble classifiers. 

