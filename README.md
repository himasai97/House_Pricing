In this project, I work on the House pricing problem from Kaggle using the Ames Housing dataset, compiled by Dean De Cock. With 79 explanatory variables describing (almost) every aspect of residential homes in Ames, Iowa, the aim is to predict the final price of each home.

As part of this project, I covered the following machine learning techniques:

### (1) Exploratory Data Analysis

Here I first looked at the statistical properties of the data and the existing relationship between different feature variables. 

Based on this information, I analyzed the missing values present in each of the feature variables and designed appropriate algorithms for handling such missing data. 

After ensuring there are no missing values in the data, I have then developed algorithms for encoding categorical features based on their properties.

### (2) Pre-processing steps in the Pipeline

In the pre-processing steps, some of the transformations applied custom logic. As a result, I have created custom transformers from scratch, to be included in the Pipeline. 

For some of the transformations that are only applied to specific feature variables, like one hot encoding for categorical features, I have used ColumnTransformer as it allows different columns of the input to be transformed separately.

### (3) Model Development

For regression, I used XGBRegressor and obtained optimal parameters for this model using GridSearchCV method. The performance of the model is evaluated using RMSE score with cross-validation.

Inspired by: [Erik Bruin's Kaggle notebook](https://www.kaggle.com/erikbruin/house-prices-lasso-xgboost-and-a-detailed-eda/report) 

