
# Churn Prediction

The business objective was to predict whether the customers are likely to churn or not. Here a churned customer means he provides less or zero revenue and increases the competitor market share. The dataset had 7043 rows and 24 columns.

For EDA, please refer to : Churn Analysis - EDA.ipynb

For Model Building, please refer to: Churn Analysis - Model Building.ipynb

For Model Deployment- app.py
## API Reference

https://telecom-churn-prediction-api.herokuapp.com
## Overview

![App Screenshot](https://github.com/Naveen-Gowda-2525/Churn-Prediction/blob/main/Images/Telco1.JPG?raw=true)
![App Screenshot](https://github.com/Naveen-Gowda-2525/Churn-Prediction/blob/main/Images/Telco2.JPG?raw=true)
![App Screenshot](https://github.com/Naveen-Gowda-2525/Churn-Prediction/blob/main/Images/Telco3.JPG?raw=true)
![App Screenshot](https://github.com/Naveen-Gowda-2525/Churn-Prediction/blob/main/Images/Telco4.JPG?raw=true)

## Data Processing,EDA and Feature Engineering
The dataset was first cleaned and a detailed end to end exploratory data analysis was performed and the characteristics  of the customers that are more likely to churn were found out. Various visualizations were drawn using seaborn and matplotlib libraries. The major insights that were drawn from EDA are-
  
  •	Electronic check medium are the highest churner.
  
  •	Contract Type - Monthly customers are more likely to churn because of no contract terms, as they are free to go customers.
  
  •	No Online security, No Tech Support category are high churners.
  
  •	Non senior Citizens are high churners.

After the EDA all the categorical variables were converted into numeric variables with the help of dummy variables. 
The dataset was also checked if it was balanced or not and it was found to be imbalanced so in order to fix this over sampling by smote was implemented to fix it.

## Model Building

A classification model was built by splitting the dataset into test and train dataset and finding the right hyper parameters in order to avoid the problem of overfitting.
After trying out with different classification models random forest was found to be the best  model as it gave an accuracy of 95%.
The model was deployed with flask framework and Flask API was created using heroku.

![App Screenshot](https://github.com/Naveen-Gowda-2525/Churn-Prediction/blob/main/Images/Screenshot%202021-11-10%20at%2019-22-50%20Naveen-Gowda-2525%20Churn-Prediction%20The%20business%20objective%20was%20to%20predict%20whether%20the%20cust%5B...%5D.png?raw=true)

## Deployment

![App Screenshot](https://github.com/Naveen-Gowda-2525/Churn-Prediction/blob/main/Images/Telco6.JPG?raw=true)
