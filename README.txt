# Churn-Prediction
The business objective was to predict whether the customers are likely to churn or not. Here a churned customer means he provides less or zero revenue and increases the competitor market share. The dataset had 7043 rows and 24 columns.
The dataset was first cleaned and a detailed end to end exploratory data analysis was performed and the characteristics  of the customers that are more likely to churn were found out. Various visualizations were drawn using seaborn and matplotlib libraries. The major insights that were drawn from EDA are-
  •	Electronic check medium are the highest churner.
  •	Contract Type - Monthly customers are more likely to churn because of no contract terms, as they are free to go customers.
  •	No Online security, No Tech Support category are high churners
  •	Non senior Citizens are high churners
After the EDA all the categorical variables were converted into numeric variables with the help of dummy variables. 
The dataset was also checked if it was balanced or not and it was found to be imbalanced so in order to fix this over sampling by smote was implemented to fix it. A classification model was built by splitting the dataset into test and train dataset and finding the right hyper parameters in order to avoid the problem of overfitting.
After trying out with different classification models random forest was found to be the best  model as it gave an accuracy of 92%.
The model was deployed with flask framework and Flask API was created using heroku.

For EDA, please refer to : Churn Analysis - EDA.ipynb
For Model Building, please refer to: Churn Analysis - Model Building.ipynb
For Model Deployment- app.py
Flask Api - https://telecom-churn-prediction-api.herokuapp.com
