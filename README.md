# Cross Selling Vehicle Insurance
 Building an ML Model to identify prospective vehicle insurance buyers.

This is a Machine Learning Task involving creation of a ML Model in order to employ the marketing strategy of cross selling. Cross Selling involves the attempt to sell new product or service to existing customers of an organization, who buy similar products or services. In this business case, a dataset consisting of health insurance holders is provided. The objective of the task is to identify which health insurance holders could be prospective vehicle insurance buyers.

The dataset has been uploaded by Amol Kumar on Kaggle. Find the link here - https://www.kaggle.com/anmolkumar/health-insurance-cross-sell-prediction

The several activities carried out during the task are as follows - 

### Data Cleaning 
- Issues with found with categories names and names of columns in dataset
- Also, several categorical features wrongly identified as numerical features.


### Exploratory Data Analysis
- Univariate Analysis was performed to understand characteristics of the independent features and target.
- Bi-variate Analysis performed to understand the relationship between the predictors and the target and which features are important / not important for predicting prospective buyers.
- Multivariate Analysis performed to understand the interaction between multiple variables and understand how they help in differentiating between classes.
- Key Inisights : Imbalance in target classes identified, Age and Gender of insurance holders, age of vehicle, previous damages, insurances, region and sales policy contribute in seperating classes, no pair of numerical features have any correlation between themselves or help in seperating classes.
- Data Not linearly seperable.

## Data Preprocessing
- No missing values in the dataset and no outliers in remaining numerical features.
- Data was split into train and test before proceeding to prevent data leakage.
- One Hot Encoding performed to encode categorical features.

## Model Building
- Logistic Regression, Bernoulli Naive Bayes, Decision Tree and several ensemble techniques used.
- Poor Results obtained due to imbalance in target classes.
- Oversampling technique SMOTE employed on training sample to improve learning ability of models.
- Boosting techniques perform poorly, no improvement in naive bayes but tree based models show good scores.
- Decision Tree selected based on train, test and cross validation scores.
- Feature Selection and Parameter tuning adopted to improve baseline models.
- Final Model achieves accuracy of 0.76, 0.65 macro F1, 0.45 f1 and 0.846 auc score on test sample.
