# What Drives the Price of a Car?
Here is link to the notebook  - https://github.com/Mawitey/RA11_1/blob/main/model%20for%20used%20cars.ipynb

###  Problem statement
Here the dealership is trying to identify what factors make a car more or less expensive, Out of the given 426K car I have dropped some records with missing values and I am considering car prices of more than $0 prices since the project is for dealership. 

### Results
From our model, I picked the top 50 of the results to look into. To start with the year of the car, for every new car (meaning increase in the year) the car price increase by $3814.14 dollars so the dealer needs to have more newer car for more revenue. On the other hand the milage is inversely proportional with the price, meaning for every milage that increased the price decreased by $2909.25, so the dealership needs to have less milage cars for better profit. When we see the cyliders, higher cyliders (12, 8) seem to have increase in price, cars which take diesel and electric cars also make the price of the car increase. On title 'parts only' seems to increase the price significantly while on transmission both automatic and manual increase the value of the car. When we see the size of the car, full-size cars have higher value and on type of cars trucks seem to have more value. Based on the above recommendation the dealership can refine it's inventory. 

### Findings
For this assessment, I have picked feature like condition, cylinders, fuel, title_status, transmission, size, type as a primary factors for car prices. I have dropped id because it might not be relevant to the price of the car and I believe the remaining feature were not that important also for target I have picked price. For this initial model, data is split to 80/20 train/test split and I have used Linear regression, ridge and lasso for modeling. Standard scaler is used to scale on numeric data and OneHotEncoder is used for categorial data. I have printed the coefficient to see the results for each feature and RMSE (Root Mean Squared Error) for evaluating the error of our model with the actual data. In this case, I have also add the RMSE of the lasso model with grid search and cross validation, and all models have similar RMSE results. On average, what the model predicted and the actual prices are different by 9686.67

### Next steps
Next I will try to include all the remaing features like region, manufacturer, model, VIN, drive, paint_color and state and determine how these values affect the price of a car.
