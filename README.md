# Credit_Risk_Analysis

## Project Overview
The purpose of this project is to build and evaluate several machine learning models to predict credit risk.  Using Python, we adopted the following procedures:

- Oversample the data using the RandomOverSampler and SMOTE algorithms.
- Undersample the data using the ClusterCentroids algorithm.
- Use a combination of over- and undersampling using the SMOTEENN algorithm.
- Compare two machine learning models that reduce bias - BalancedRAndomForestClassifier and EasyEnsembleClassifier.

## Results

### RandomOverSampler Model

![image](https://user-images.githubusercontent.com/78937719/124356883-3e565500-dbde-11eb-97dc-ab8e22391ebf.png)

- The balanced accuracy score is 65%.
- The high risk precision is 1% with 63% sensitivity which makes an F1 of 2%.
- The low risk population's precision nears 100% with a sensitivity of 66%.

### SMOTE Model

![image](https://user-images.githubusercontent.com/78937719/124357033-04d21980-dbdf-11eb-8c86-19773530d4f9.png)

- The balanced accuracy score is 63%.
- The high risk precision is 1% with a 60% sensitivity which makes an F1 of 2%.
- The low risk population precision nears 100% with a sensitivity of 66%.

### ClusterCentroidsModel

![image](https://user-images.githubusercontent.com/78937719/124357189-d99bfa00-dbdf-11eb-9c10-2a50b7e64080.png)

- The balanced accuracy score is 51%.
- The high risk precision is 1% with a 59% sensitivity which makes an F1 of 1%.
- The low risk population precision nears 100% with a sensitivity of 43%.

### SMOTEENN Model

![image](https://user-images.githubusercontent.com/78937719/124357294-6777e500-dbe0-11eb-8d1a-0b0a3223f665.png)

- The balanced accuracy score is 63%.
- The high risk precision is 1% with a 72% sensitivity which makes an F1 of 2%.
- The low risk population precision nears 100% with a sensitivity of 53%.

### BalancedRandomForestClassifier Model

![image](https://user-images.githubusercontent.com/78937719/124357423-07ce0980-dbe1-11eb-84a7-831b1ee017ff.png)

- The balanced accuracy score is 79%.
- The high risk precision is 4% with a 67% sensitivity which makes an F1 of 7%.
- The low risk population precision nears 100% with a sensitivity of 91%.

### EasyEnsembleClassifier Model

![image](https://user-images.githubusercontent.com/78937719/124357522-87f46f00-dbe1-11eb-838e-07835cbc6ea7.png)

- The balanced accuracy score is 93%.
- The high risk precision is 7% with a 91% sensitivity which makes an F1 of 14%.
- The low risk population precision nears 100% with a sensitivity of 94%.

## Summary
- Each of the models used to perform the credit risk analysis demonstrate weak precision in determining high credit risk.
- The Ensemble models fared better especially on the sensitivity of high risk credit.
- The EasyEnsembleClassifier Model shows a recall of 94% which demonstrates that it detects almost all high risk credit, but with a such a low precision a lot of low credit risks are falsely detected as high risk which would hurt the banks credit strategy and revenue by missing those opportunities.

For the reasons summarized, it would not be recommended that the bank use any of these models to predict credit risk.

