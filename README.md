# Credit_Risk_Analysis

## Overview
Using Python and several machine learning models, predict the credit risk.

## Resources
* Data Source: LoanStats_2019Q1.csv
* Software: Jupyter Notebook 6.3.0(Running on: Python 3.7.10, Anaconda 4.10.3)

## Results
### RandomOverSampler model

* The balanced accuracy score is 65%
* The high_risk precision is about 1% only with 69% sensitivity with F1 of 2% only.
* Due to high number of low_risk population (17104), its precision is almost 100% with a sensitivity of 60%

### SMOTE model

* The balanced accuracy score is 66%
* The high_risk precision is about 1% only with 63% sensitivity with F1 of 2% only.
* Due to high number of low_risk population, its precision is almost 100% with a sensitivity of 69%

### ClusterCentroids model

* The balanced accuracy score is 66%
* The high_risk precision is about 1% only with 69% sensitivity and F1 of 1% only.
* low_risk precision is almost 100% with a sensitivity of 40%

### SMOTEENN model

* Balanced accuracy score is 65%
* The high_risk precision is about 1% with 72% sensitivity and F1 of 2%
* low_risk precision is almost 100% with a sensitivity of 57%

### BalancedRandomForestClassifier model

* Balanced accuracy score is 78%
* high_risk precision is about 4% with 66% sensitivity and F1 of 7%
* low_risk precision is almost 100% with a sensitivity of 89%

### EasyEnsembleClassifier model

* Balanced accuracy score is 92%
* high_risk precision is about 9% with 89% sensitivity and F1 of 16%
* low_risk precision is almost 100% with 94% precision


## Summary

All models used for the credit risk analysis show weak precision in determining if a credit risk is high.
Ensemble model shows the most improvement on the sensitivity of the high risk credits.
EasyEnsembleClassifier model shows a score of 92% so it will detect almost all high risk credit but due to the low precision, a lot of low risk credits are still falsely detected as high risk which could result in credit rejected for low risk accounts.
Due to the above analysis, it can be stated that none of these models would be recommended for the use to predict credit risk

