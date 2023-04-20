# HepatitisC-Predictions
Yi Ren

## Data
The dataset used in this project is [HCV](https://archive.ics.uci.edu/ml/datasets/HCV+data), which contains the laboratory values of blood donors and Hepatitis C patients with their demographic values. All attributes except Category and Sex are numerical. The laboratory data are the attributes 5-14:

+ X (Patient ID/No.)
+ Category (diagnosis) (values: '0=Blood Donor', '0s=suspect Blood Donor', '1=Hepatitis', '2=Fibrosis', '3=Cirrhosis')
+ Age (in years)
+ Sex (f,m)
+ ALB
+ ALP
+ ALT
+ AST
+ BIL
+ CHE
+ CHOL
+ CREA
+ GGT
+ PROT

## Goal
The target attribute for classification is Category: blood donors vs. Hepatitis C patients (including its progress ('just' Hepatitis C, Fibrosis, Cirrhosis). To be more specific, I combined '0s=suspect blood donors' and '0=blood donors' as blood donors. And I combined the category of '1=Hepatitis', '2=Fibrosis' and '3=Cirrhosis' as 1 to represents the patient is Hepatitis C patients.

The main goal for this project is to predict whether the patient has Hepatitis C or not (binary response) using the given HCV data:
+ Used pipeline and cross validation to choose your best model for each model type. 
+ Performed transformations using the functions from MLlib and evaluate the best models using AreaUnderROC and AreaUnderPR metrics.
 
