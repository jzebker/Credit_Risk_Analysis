# Credit_Risk_Analysis
## Overview
Apply machine learning to calculate credit risk using LendingClub data.  First, oversample the data using the RandomOverSampler and SMOTE algorithms and undersample the data using the ClusterCentroids algorithm. Then, use a combinatorial approach of over and undersampling using the SMOTEENN algorithm.  Next, compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier. Finally, evaluate the performance of these models and make a recommendation on whether or not they should be used to predict credit risk.
## Results
### RandomOverSampler
• Balanced accuracy score - 0.6468035260322871

• Precision score

• Recall score

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportROS.png?raw=true"></p>

### SMOTE
• Balanced accuracy score - 0.6268900250190362

• Precision score

• Recall score

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportSMOTE.png?raw=true"></p>

### ClusterCentroids
• Balanced accuracy score - 0.5276236750184319

• Precision score

• Recall score

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportCC.png?raw=true"></p>

### SMOTEEN
• Balanced accuracy score - 0.6459876878945736

• Precision score

• Recall score

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportSMOTEEN.png?raw=true"></p>

### BalancedRandomForestClassifier
• Balanced accuracy score - 0.7223743105664133

• Precision score

• Recall score

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportBRFC.png?raw=true"></p>

### EasyEnsembleClassifier
• Balanced accuracy score - 0.7499425891680869

• Precision score

• Recall score

• Full scikit report

<p align="center"><img src="https://github.com/jzebker/Credit_Risk_Analysis/blob/main/img/imbClassReportEE.png?raw=true"></p>

## Summary

