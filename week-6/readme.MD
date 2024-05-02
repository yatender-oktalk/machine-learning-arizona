# Abstract

The project was conducted on the German Credit Data with the purpose of exploring,
processing and ultimately developing a machine learning model for predicting the Risk
assessment for a given applicant. The dataset was explored to point out useful relationships
between variables for future preprocessing steps, starting from the missing value treatment
evaluations. Preparing both the categorical and numerical variables for the Machine Learning
algorithms; missing values were imputed, numerical variables were Log-Scaled, Standardized
and Clustered while categorical variables were One-Hot Encoded.


In the Machine Learning phase of the project for the preprocessed dataset; K-Nearest Neighbors
(KNN), Decision Trees (DT), Logistic Regression (LR), Multilayer Perceptrons (MLP) and
Support Vector Machines (SVM) models were implemented with hyper-parameter tuning via
cross validation and the accuracies of each trained model was compared. The Logistic
Regression (LR) model yielded the highest accuracy score of, exceeding other alternatives when
considering other metrics such as F1-Score, which are further discussed in the report.


In order to test the limit in which the accuracy of the Logistic Regression model can be
improved, Feature Engineering methods were implemented by further investigating correlations
between the variables. After feature extraction and selection trials, a Logistic Regression model
with only 
['Checking account_Unknown', 'Checking account_little', 'credit_per_duration', 'Saving accounts_little']
 variables were trained and tested, yielding a _79% accuracy score model_ as the
finest model developed during the project.


# Introduction

The task is to create a Machine Learning model that can predict the credit risk assessment for a
given application. Due to the binary nature of the prediction (good or bad), this is a Binary
Classification problem consisting of 3 numerical variables and 6 categorical variables, excluding
the target column. The need for combining these fundamentally different variables and exploring
hidden relationships between them, make all following steps equally crucial and relevant.

##### 1-) Exploratory Data Analysis

##### 2-) Data Preprocessing

##### 3-) Machine Learning (including Feature Engineering) 

