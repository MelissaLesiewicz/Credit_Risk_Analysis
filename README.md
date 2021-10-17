# Credit_Risk_Analysis
## Overview
### Project:
The purpose of this project is to create a reliable credit risk evaluation model. Given a dataset from LendingClub, a peer-to-peer lending services company, we know if a loans current status is Current, 16-30 days late, 31 - 120 days lates,
In Grace Period, or in Default. Using several variables known about the given borrowers I created and evaluated 6 different models to determine which model would be the best model to evaluate credit risk of future applicants.
### Project Details:
All loans in the given dataset with a loan status of Current were evaluated as low risk and any loan with a loan status of Late, in grace period, or Default were considered high risk. Loan amount, interest rate, number of installments, home ownership, annual income, debt-to-income ration, and several other factors were used as variables to create the 6 models.

## Results:

### Types of Models Created:
*  Random Oversampling (RO)
*  SMOTE Oversampling (SO)
*  Cluster Centroids (CC)
*  SMOTEENN (SM)
*  Balanced Random Forest Classifier (BRF)
*  Easy Ensemble Classifier (EE)

### Precision for Each Model:

Model | High-Risk | Low-Risk
 --- | --- | ----
RO: | .008 | .997
SO: | .009 | .998 
CC: | .009 | .998
SM: | .008 | .998
BRF:| .035 | .998
EE: | .087 | .999

### Sensitivity for Each Model

Model | High-Risk | Low-Risk
--- | --- | ---
RO: | .603 | .662
SO: | .667 | .690
CC: | .667 | .690
SM: | .718 | .567
BRF: |.635 | .902
EE:  |.875 | .948

### Balanced Accuracy Score for Each Model
*  RO:   .632
*  SO:   .678
*  CC:   .632
*  SM:   .642
*  BRF:  .769
*  EE:   .912

### Easy Ensemble Classifier Results Screen Image
![EasyEnsembleClassifier](https://user-images.githubusercontent.com/86027932/137642995-11f0c27a-55e3-4684-b89a-fd23b9d8775e.png)


## Summary
The Easy Ensemble Classifier model has the best overall results. This model had the highest balanced accuracy Score at 91.2%, the highest precision and sensitivity rate of determining both high and low risk loans. While the model isn't perfect I would recommend using this method. I think it sufficiently reduces the risk of approving loans that will potentially default while also limiting the error of falsely identifying a loan as high-risk so the club doesn't lose out out on too much interest income. I would suggest trying this method with scaled data and various estimators before going ahead with this specific model. 
 

