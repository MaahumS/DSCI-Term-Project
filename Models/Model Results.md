## Overview of Each Model
Each model reads the excel input, sets our target variable, selects our desired attributes (based on our data exploration results), 
converts all variables from nominal to numerical, and splits data into two groups; training and validation. 
The desired model type (K-NN, random forest, or linear regression) is then performed on the training group & a regression performance 
operator is applied to both the training and validation groups so that we can evaluate how our model performed.
We performed this model multiple times with different numbers of trees and compared the root mean squared error (RMSE) and R2 of our 
validation group. 

## Random Forest Model Results
When no variables are excluded the optimal number of trees is 45 where RMSE is minimized at 3166.227 and R2 is maximized at 0.733. 
When some variables are excluded, the optimal number of trees is 75 where RMSE is minimized at 3120.021 and R2 is maximized at 0.742. 
When our model has fewer attributes, more trees are required to accurately capture the relationships between variables.

## K-NN Model Results
The optimal value of k is 20 as this value minimizes RMSE at 3928.514 and maximizes R2 at 0.616.  
This tells us that there is no underfitting or overfitting occurring.  

## Linear Regression Results
Our best-performing model occurs when only Known Allergies is excluded as our RMSE is minimized at 3984.241 and our R2 is maximized 
at 0.575. This tells us that known allergies may be introducing unnecessary variation to our model. This also tells us that Weight 
and History of Diabetes may be positive contributions to the model's performance as the RMSE increased and R2 decreased when these 
variables were removed. The correlation matrix shows us that the variable Age has a strong positive correlation with 
insurance premium price and the variable Known Allergies has a very weak correlation to premium price, as confirmed by our model. 
