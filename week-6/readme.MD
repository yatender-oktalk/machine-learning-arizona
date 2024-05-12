# Loan Default Prediction Project:
- This project aims to build a machine learning model for predicting whether a customer will default on a loan based on historical data.
- The project follows a structured approach, including data exploration, visualization, and the application of various machine learning models.
- The ultimate goal is to create a publishable and reproducible project that showcases the process of developing a predictive model for loan default prediction.


## Project Organization - The project is organized into the following main steps:

### 1.) Data Understanding and Cleaning:
- Read and understand the dataset's contents and column descriptions.
- Perform summary statistics analysis for numerical and categorical columns.
- Check for missing values and duplicates.
- Impute missing data where necessary.

### 2.) Data Visualization:
- Visualize the distribution of numerical features using histograms, density plots, and boxplots.
- Explore correlations between numerical features using a pairplot and heatmap.
- Analyze categorical features using count plots with and without 'default' as the hue.


### 3.) Machine Learning Models:
- Identify the target variable ('default') and predictor variables (numerical and categorical).
- Encode nominal columns using one-hot encoding and ordinal columns using ordered ranking.
- Apply standard scaling to numerical features using the Standard Scaler.
- To scale I have utilized the log scaling for numerical values for better fit.
- Split the data into training and testing sets with stratification.
- Hyperparameter tune machine learning models using GridSearch and cross-validation.
- Fit all the models on the training set and evaluate performance on testing set.
- Compare models using AUC-PR and ROC curves along with AUC values from different values of thresholds.
- Finalize the model with the help of AUC-PR values and find a custom threshold to achieve optimal recall performance.

## Repository Structure:

#### Dataset: Contains the dataset files used in the project.
- bank-data.csv: Original dataset. This is the default dataset which we will use.

#### Dataset generated while execution
- m-1.csv this dataset contains almost similar data but just some typo fixed.
- m-2.csv this dataset is when we treat the categorical & ordinal data.
- feature-scaled.csv this dataset contains the final dataset which is feature scaled, treated categorical and ordinal data and missing value treatment. This dataset is fit to create model and it also has some feature engineering.

#### ipynb project files
##### 2.) ipynb files: Contains Jupyter notebooks for each project step.
- project_part_1_data_exploration.ipynb: Data exploration and 
- project_part_2_model_creation.ipynb: Data cleaning & Application of machine learning models.

### 3.) Readme file: 
Contains the project README file.
- README.md: Detailed project overview and instructions.

```
Loan_Default_Prediction_Project/
│
├── CSV datafiles/
│   ├── bank_data.csv              # Original dataset
│
├── Jupyter notebooks/
│   ├── project_part_1_data_exploration.ipynb           # Data exploration 
│   ├── project_part_2_model_creation.ipynb   # Data cleaning & Machine learning modeling
│
│
└── README.txt				     # Project README file
```

### Getting Started:
- Install the required libraries and dependencies listed in the project environment.
- Run the Jupyter notebooks in the notebooks/ directory in the specified order to follow the project steps.
- Explore the data, visualizations, and model evaluations as presented in the notebooks.

Necessary Python Libraries - The project requires the following Python libraries:
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- jupyter
- xgboost


### Conclusion:
- The project demonstrates a comprehensive approach to building and evaluating machine learning models for loan default prediction.
- Following the provided steps and exploring the notebooks, one can gain insights into the data, model performance, and strategies for improving recall in imbalanced classification scenarios.