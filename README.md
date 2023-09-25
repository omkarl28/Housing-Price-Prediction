# House Price Prediction : Advanced Regression
> A US-based housing company named Surprise Housing has decided to enter the Australian market.
> The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price.

## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)


<!-- You can include any other section that is pertinent to your problem -->

## General Information
- Provide general information about your project here.

- What is the background of your project?
> A US-based housing company named Surprise Housing has decided to enter the Australian market.
> The company uses data analytics to purchase houses at a price below their actual values and flip them on at a higher price.

- What is the business problem that your project is trying to solve?
> The company is looking at prospective properties to buy to enter the market.
> You are required to build a regression model using regularisation in order to predict the actual value of the prospective properties   and decide whether to invest in them or not.
> The company wants to know:
>Which variables are significant in predicting the price of a house, and
> How well those variables describe the price of a house.
Also, determine the optimal value of lambda for ridge and lasso regression.

- What is the dataset that is being used?
> Data Set is available in a CSV file named train.csv

- Objective of the Project?
> You are required to model the price of houses with the available independent variables.
> This model will then be used by the management to understand how exactly the prices vary with the variables.
> They can accordingly manipulate the strategy of the firm and concentrate on areas that will yield high returns.
> Further, the model will be a good way for management to understand the pricing dynamics of a new market.

- Approach to solve this business problem
> Step 1 : Data Understanding and Exploratory Data Analysis ( EDA )
> Step 2 : Data Preperation
> Step 3 : Training the model
> Step 4 : Model Prediction and Evaluation
> Step 5 : Redge and Lasso Regularization
> Step 6 : Conclusions and Results

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->

## Conclusions
- The optimal value of LAMBDA we got in case of Ridge and Lasso is :
- Ridge - **2.0**
- Lasso - **0.0001**
- The r2 value we got in case of Ridge and Lasso is:
- Ridge - Train = **0.930** , Test = **0.896**
- Lasso - Train = **0.927** , Test = **0.902**
- The Mean Squared error in case of Ridge and Lasso is:
- Ridge - **0.00297**
- Lasso - **0.00280**
- - We can clearly observe that the Mean Squared Error of Lasso is slightly lower than that of Ridge.
- Also since Lasso helps in feature reduction (as the coefficient value of one of the lasso's feature to be shrunk toward 0) and helps to increase model interpretation by taking the magnitude of the coefficients thus **Lasso has a better edge over Ridge.**

<!-- You don't have to answer all the questions - just the ones relevant to your project. -->


## Libraries Used
- import pandas as pd #Data Processing
- import numpy as np #Linear Algebra
- import seaborn as sns #Data Visualization
- import matplotlib.pyplot as plt #Data Visualization
- import warnings #Warnings
- warnings.filterwarnings ("ignore") #Warnings
- import sklearn
- from sklearn.model_selection import train_test_split #for spliting the data in terms of train and test
- from sklearn.preprocessing import MinMaxScaler #for performing minmax scaling on the continous variables of training data
- from sklearn.feature_selection import RFE #for performing automated Feature Selection
- from sklearn.linear_model import LinearRegression #to build linear model
- from sklearn.linear_model import Ridge #for ridge regularization
- from sklearn.linear_model import Lasso #for lasso regularization
- from sklearn.model_selection import GridSearchCV #finding the optimal parameter values
- from sklearn.metrics import r2_score #for calculating the r-square value
- import statsmodels.api as sm #for add the constant value
- from sklearn import metrics
- from statsmodels.stats.outliers_influence import variance_inflation_factor #to calculate the VIF
- from sklearn.metrics import mean_squared_error #for calculating the mean squared error

<!-- As the libraries versions keep on changing, it is recommended to mention the version of library used in this project -->


## Contact
Created by [@omkarl28] - feel free to contact me!


<!-- Optional -->
<!-- ## License -->
<!-- This project is open source and available under the [... License](). -->

<!-- You don't have to include all sections - just the one's relevant to your project -->
