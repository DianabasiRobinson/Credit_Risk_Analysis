# Credit_Risk_Analysis
Supervised Machine Learning and Credit Risk
## Project Overview
Credit Risk Analysis is created to analyze credit card risk by employing different techniques to train and evaluate models with unbalanced classes: oversampling with RandomOverSampler and SMOTE algorithms, and undersampling the data using the ClusterCentroids algorithm, then using a combinatorial approach of over- and undersampling using the SMOTEENN algorithm. And after that compare two new machine learning models that reduce bias, BalancedRandomForestClassifier and EasyEnsembleClassifier, to predict credit risk.

## Results
- Naive Random Oversampling balanced accuracy score and imbalanced classification report:

![Imbalanced](https://user-images.githubusercontent.com/109990578/209365404-1c07a334-c2bc-4dc0-af30-1327736eb8ef.png)

-SMOTE Oversampling balanced accuracy score and imbalanced classification report:

![SMOT_balanced](https://user-images.githubusercontent.com/109990578/209365925-475fcd55-1e12-4ae0-9f38-9809e8442d35.png)

- Undersampling balanced accuracy score and imbalanced classification report:

![undersampling imbalanced](https://user-images.githubusercontent.com/109990578/209366154-98c6c78c-6e0d-4f6f-99f4-d10969702661.png)

- Combination (Over and Under) Sampling balanced accuracy score and imbalanced classification report:

![bal imbal](https://user-images.githubusercontent.com/109990578/209366462-591abfea-9075-4bdb-a7f4-cafa0087d51a.png)

- Balanced Random Forest Classifier balanced accuracy score and imbalanced classification report:

![Random forest](https://user-images.githubusercontent.com/109990578/209366920-dbb41b41-f94f-4c07-b1f0-512de05169d2.png)

- Easy Ensemble AdaBoost Classifier balanced accuracy score and imbalanced classification report:

![Ensemble Adaboost](https://user-images.githubusercontent.com/109990578/209366994-d91a5453-29a5-449b-b91d-922422e7f7b9.png)

## Summary
- The Combination (Over and Under) Sampling showed better balanced accuracy score - about 68% (against random oversampling 65%, SMOTE oversampling 66% and undersampling 64.4%).
- However the Easy ensemble classifier model got higher balanced accuracy score (93%) than balanced random forest classifier (79%).Thus both classification models performed better accuracy score than sampling models.
- F1 score is highest for Easy Ensemble AdaBoost Classifier - 97%
- All the models show much more false-positive over true-positive results which means a lot of customers' credit cards will be restricted for no reason.
- These models is not suitable for commercial use and further consideration/processing should be done in case the model was partially used in the decision-making process.
