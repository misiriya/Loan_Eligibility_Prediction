# Bank Loan Eligibility Prediction:  
This notebook was created as part of my project for the Kaggle BIPOC program. This project is based on Predicting Approvals for Banking Loans. I decided to work on the U.S. Small Business Administrations Loan datasets, which are freely available online. So, we will see here, how to deal with Loan Approval Predictions using Machine Learning in Python.

## Project Overview 
* Built a tool to understand the past customers' profile in order to minimize the risk of future loan defaults and loan eligibility
* Cleaned dataset and use Feature Selection Method
* Tried models like Decision Tree Classifier,Support Vector Machine, Logistic Regression and Naive Bayes Classifier and chose best one using K-Fold Cross-Validation
* Visualized confusion matrix to evaluate the performance of model

## Code and Resources Used
* Python Version: 3.7  
* Packages: pandas, numpy, sklearn, matplotlib,seaborn, pandas_profiling,
* Link to Dataset: https://drive.google.com/open?id=1mrKSmWdOZnAI59jaRYEgS99zQJF8pOZg
* Dataset: https://data.world/nerb/sba-loan-guarantee-data/workspace/file?filename=7a_504_FOIA%2520Data%2520Dictionary.xlsx
* https://www.analyticsvidhya.com/blog/2022/05/loan-prediction-problem-from-scratch-to-end/
* https://towardsdatascience.com/exploratory-data-analysis-in-python-a-step-by-step-process-d0dfa6bf94ee
* https://www.kdnuggets.com/2021/05/deal-with-categorical-data-machine-learning.html
* https://towardsdatascience.com/predict-loan-eligibility-using-machine-learning-models-7a14ef904057
* https://www.aboutdatablog.com/post/splitting-your-data-to-fit-any-machine-learning-model
* https://www.kaggle.com/code/prashant111/naive-bayes-classifier-in-python
* https://www.kaggle.com/code/gigikenneth/eng-hau-notebook/notebook

## Project structure
The project divides into two categories:
* Data Wrangling: Cleansing and Feature Selection
* Machine Learning: Predictive Modelling

## Data Wrangling: Cleansing and Feature Selection
There was need to clean dataset so that it was useable for our model. I made the following changes and created the following variables:
* Added a column for if the loan was in default, based on LoanStatus variable values and named it Defaulter
* Checked if data is duplicated and removed them
* Removed columns those had highest percentage of missing values
* Imputed missing values of different types of colummns by building pipelines for each
* Converted the categorical variables into dummy variables

## Machine Learning: Predictive Modelling
* Split the data into train and tests sets with a test size of 20% and 30% alternatingly.
* Tried different models like Decision Tree Classifier,Support Vector Machine, Logistic Regression and Naive Bayes Classifier
* Evaluated them using K-Fold Cross-Validation by comparing algorithms
* Best performed model: Decision Tree Classifier

## Model Performance
* The metrics used for the models’ evaluation are the accuracy and confusion matrix 
