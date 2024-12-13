# Summary of Visualizations
Before we created our model, we first wanted to understand our dataset. 
From our data dictionary, we found our dataset has a mix of both categorical and numerical predictor variables.
However, not all these variables affect our target variable. 
As such, we created the following visualizations to help determine what predictors to include in our dataset.

## Findings
- Average premium price for those with 2 or 3 surgeries is higher than those with 0 or 1 surgeries.  
- People with a history of chronic diseases have a slightly higher average premium price than those with no history of chronic diseases. 
- People who have had prior transplants have a noticeably higher average premium price than those with no prior transplants. 
- Age vs average premium price scatterplot shows a positive correlation between age and premium price.
This plot has an R-squared value of 0.8188 which tells us that 81.88% of the variation in premium price can be explained by age.  
- Weight vs average premium price scatterplot shows no correlation between weight and premium price. This plot has an R-squared value of 
0.0347 which tells us weight does not explain any variation in our data set. 
- History of diabetes vs average premium shows almost no difference in average premium price for those with or without a history of diabetes. 
- History of known allergies vs average premium shows almost no difference in an average premium price for those with or without known allergies.

## Conclusion: 
Our model will consider predictors like number of surgeries, history of chronic disease, history of transplants, history of cancer, 
history of blood pressure, and age. Our model will not consider predictors like weight, history of diabetes, and known allergies.   

