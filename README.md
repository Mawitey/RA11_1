# What Drives the Price of a Car?
Here is link to the notebook  - https://github.com/Mawitey/RA11_1/blob/main/prompt_II_(8)%20(2).ipynb

###  Problem statement
Here the dealership is trying to identify what factors make a car more or less expensive, Out of the given 426K car I have dropped some records with missing values and I am considering car prices of more than $0 prices since the project is for dealership. 

### Results
Based on our model, the primarly factors that influenced car prices are year and milage(odometer) because they were given in numbers (id is also given in number but I have dropped it since it can not be used as a factor for car price). For every new car (meaning increase in the year) the car price increase by $3559.52 dollars so the dealer needs to have more newer car for more revenue. On the other hand the milage is inversely proportional with the price meaning for every milage that increased the price decreased by $2620.68, so the dealership needs to have less milage cars for better profit.

### Findings
For this initial model my focus is in the top 20 of the features(since we have many features), that is year and milage(odometer) and some car from certain regions, and price as the target variable. Next data is split to 80/20 train/test split. Standard scaler is used to avoid large values from dominating the output of the model. I used Linear Regression, Ridge, and Lasso models to find the amount being increased/decreased using coefficient. RMSE (Root Mean Squared Error) is chosen for evaluation because it provides the average prediction error. The Linear Regression model achieved an RMSE of approximately 12592.38, Lasso and Ridge also gave out similar results. An RMSE of $12592.38 means that, on average, what the model predicted and the actual prices are different by $12592.38.

### Next steps
Next I will try to include how the fuel type, manufacturer, model, condition, cylinders, title status, transmission, type and size affect the price of a car.
