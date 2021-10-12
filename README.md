# Credit_Risk_Analysis
## Overview
Apply machine learning to calculate credit risk using LendingClub data.  First, oversample the data using the RandomOverSampler and SMOTE algorithms and undersample the data using the ClusterCentroids algorithm. Then, use a combinatorial approach of over and undersampling using the SMOTEENN algorithm.  Next, compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier. Finally, evaluate the performance of these models and make a recommendation on whether or not they should be used to predict credit risk.
## Results
### RandomOverSampler
• Balanced accuracy score - 0.6468035260322871

• Precision score - ***high_risk:*** .01 ***low_risk:*** 1.00

• Recall score - ***high_risk:*** .62 ***low_risk:*** .67

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportROS.png?raw=true"></p>

### SMOTE
• Balanced accuracy score - 0.6268900250190362

• Precision score - ***high_risk:*** .01 ***low_risk:*** 1.00

• Recall score - ***high_risk:*** .61 ***low_risk:*** .64

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportSMOTE.png?raw=true"></p>

### ClusterCentroids
• Balanced accuracy score - 0.5276236750184319

• Precision score - ***high_risk:*** .01 ***low_risk:*** 1.00

• Recall score - ***high_risk:*** .63 ***low_risk:*** .42

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportCC.png?raw=true"></p>

### SMOTEEN
• Balanced accuracy score - 0.6459876878945736

• Precision score - ***high_risk:*** .01 ***low_risk:*** 1.00

• Recall score - ***high_risk:*** .71 ***low_risk:*** .58

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportSMOTEEN.png?raw=true"></p>

### BalancedRandomForestClassifier
• Balanced accuracy score - 0.7223743105664133

• Precision score - ***high_risk:*** .02 ***low_risk:*** 1.00

• Recall score - ***high_risk:*** .61 ***low_risk:*** .84

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportBRFC.png?raw=true"></p>

### EasyEnsembleClassifier
• Balanced accuracy score - 0.7499425891680869

• Precision score - ***high_risk:*** .02 ***low_risk:*** 1.00

• Recall score - ***high_risk:*** .71 ***low_risk:*** .79

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportEE.png?raw=true"></p>

## Summary
None of these models were good at predicting high_risk loans and they classified almost all as low_risk.  This is an imbalanced data set and we can see from the value counts that only 347 out of 68,817 total loans (.5%) are high_risk.  The ensemble classifiers (BalancedRandomForestClassifier and EasyEnsembleClassifier) had higher balanced accuracy scores than the other 4 models.  The EasyEnsembleClassifier and the SMOTEEN algorithm had the highest recall/sensitivity scores for high_risk.

***Recommendation*** - In general, I do not recommend using any of these models for anything other than to support loan approval and they all did poorly when predicting high_risk loans.  If we assume this data set is representative of the rest of the world, we can assume these models will continue to perform poorly at predicting high_risk loans.  

I am not a lending expert nor can I predict the future.  The object of this exercise was to understand the workings of different machine learning models and to see how they apply to a real world data set.  Perhaps somebody with more domain knowledge could write a better model than my kitchen sink approach.

