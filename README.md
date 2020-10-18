# DSRPeru_imblearn
An example on how to apply an strategy to the challenge of dealing with imbalanced datasets

Step 1:
Fitting 4 models (logistic regression, svm, random fores, ann) with randomly generated imbalanced dataset. The purpose is to set a baseline to compare with. Estimating model recall using cross-validation.
-IMB CLASS-CV.ipnyb

Step 2:
Each notebook presents a different oversampling or undersampling method (or a combination of both). Each method is applied to fit each of the 4 models from step 1. Estimating model recall using cross-validation and the creatione of pipelines. 
-Random undersampling: IC_RUND.ipnyb
-SMOTE oversampling: IC_SMOTE.ipnyb
-SMOTE + Random undersampling: IC_SMOTE_RUND.ipnyb
-SMOTE + TOMEK Links: IC_SMOTE_TL.ipnyb

Step 3:
After comparing recall for all previous model+sampling combinations, we´re able to tune hyper-parameters for the top combinations. In this example, we´ll try to boost SVM and Random Forest performance. Using Grid Search to look for the best-performing parameters.
-IC_TOP_GS.ipynb

