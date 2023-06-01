# Credit_Risk_Analysis

## Project Overview
Credit risk is an inherently unbalanced classification problem, as good loans easily outnumber risky loans. Therefore, the task is to employ different techniques to
train and evaluate models with unbalanced classes. Imbalanced-learn and scikit-learn libraries are will be used to build and evaluate models using resampling.
Using the credit card credit dataset from LendingClub, a peer-to-peer lending services company, use the RandomOverSampler and SMOTE algorithms to oversample the 
data,and undersample the data using the ClusterCentroids algorithm. Then, use a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. 
Next, compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk. Once the work is
complete evaluate the performance of these models and make a written recommendation on whether they should be used to predict credit risk.

## Deliverables

### Deliverable 1: Use Resampling Models to Predict Credit Risk 
Using knowledge of the imbalanced-learn and scikit-learn libraries, evaluate three machine learning models by using resampling to determine which is better at 
predicting credit risk. First, you’ll use the oversampling RandomOverSampler and SMOTE algorithms, and then you’ll use the undersampling ClusterCentroids algorithm.
Using these algorithms, resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score,
generate a confusion matrix, and generate a classification report.

#### Naive Random Oversampling Results

![Screenshot 2023-05-31 at 6 25 25 PM](https://github.com/mdfjoseph/Credit_Risk_Analysis/assets/114943747/683b5601-3242-40c2-8787-73444044ce49)

1.  Accuracy Score of Model:  0.6494837053958125
2.  Precision:  High_risk loans are low (.01) and Low_risk loans are high (1.00)
3.  Recall:  High_risk is .63 / Low_risk is .67
4.  F1:  High_risk is .02 / Low_risk is .80

#### SMOTE Oversampling Results

![Screenshot 2023-05-31 at 6 43 28 PM](https://github.com/mdfjoseph/Credit_Risk_Analysis/assets/114943747/f90a850c-3c5e-4fa2-a38b-d6efd7c807af)

1.  Accuracy Score of Model:  0.6079978324892934
2.  Precision:  High_risk loans are low (.01) and Low_risk loans are high (1.00)
3.  Recall:  High_risk is .55 / Low_risk is .66
4.  F1:  High_risk is .02 / Low_risk is .80

#### Undersampling Results

![Screenshot 2023-05-31 at 6 46 03 PM](https://github.com/mdfjoseph/Credit_Risk_Analysis/assets/114943747/6d8c78d1-e86c-49e1-bc9a-ec7acd6c2767)

1.  Accuracy Score of Model:  0.6079978324892934
2.  Precision:  High_risk loans are low (.01) and Low_risk loans are high (1.00)
3.  Recall:  High_risk is .57 / Low_risk is .46
4.  F1:  High_risk is .01 / Low_risk is .63

### Deliverable 2:  Use the SMOTEENN algorithm to Predict Credit Risk
Use knowledge of the imbalanced-learn and scikit-learn libraries, use a combinatorial approach of over- and undersampling with the SMOTEENN algorithm to determine
if the results from the combinatorial approach are better at predicting credit risk than the resampling algorithms from Deliverable 1. Use the SMOTEENN algorithm, 
resample the dataset, view the count of the target classes, train a logistic regression classifier, calculate the balanced accuracy score, generate a confusion 
matrix, and generate a classification report.

#### Combination (Over and Under) Sampling Results

![Screenshot 2023-05-31 at 6 50 37 PM](https://github.com/mdfjoseph/Credit_Risk_Analysis/assets/114943747/6eccb3dd-36bc-4e9f-adf5-57591226238a)

1.  Accuracy Score of Model:  0.5182244139059107
2.  Precision:  High_risk loans are low (.01) and Low_risk loans are high (1.00)
3.  Recall:  High_risk is .70 / Low_risk is .58
4.  F1:  High_risk is .02 / Low_risk is .73

### Deliverable 3:  Use Ensemble Classifiers to Predict Credit Risk
Use knowledge of the imblearn.ensemble library, train and compare two different ensemble classifiers, BalancedRandomForestClassifier and EasyEnsembleClassifier, to
predict credit risk and evaluate each model. Using both algorithms, resample the dataset, view the count of the target classes, train the ensemble classifier, 
calculate the balanced accuracy score, generate a confusion matrix, and generate a classification report.

#### Balanced Random Forest Classifier Results

![Screenshot 2023-05-31 at 6 55 35 PM](https://github.com/mdfjoseph/Credit_Risk_Analysis/assets/114943747/cd458a08-27ed-45d7-bc53-41fa15fc7c4a)

1.  Accuracy Score of Model:  0.7877672625306695
2.  Precision:  High_risk loans are low (.04) and Low_risk loans are high (1.00)
3.  Recall:  High_risk is .67 / Low_risk is .91
4.  F1:  High_risk is .07 / Low_risk is .95

#### Easy Ensemble AdaBoost Classifier

![Screenshot 2023-05-31 at 6 57 34 PM](https://github.com/mdfjoseph/Credit_Risk_Analysis/assets/114943747/ea7b493b-512d-4b62-819a-18477f8e9548)

1.  Accuracy Score of Model:  0.925427358175101
2.  Precision:  High_risk loans are low (.07) and Low_risk loans are high (1.00)
3.  Recall:  High_risk is .91 / Low_risk is .94
4.  F1:  High_risk is .14 / Low_risk is .97

## Summary

Out of all of the machine learning models I chose the Easy Ensemble AdaBoost Classifier model because it had the best accuracy score of .93 and the highest recall 
score.










