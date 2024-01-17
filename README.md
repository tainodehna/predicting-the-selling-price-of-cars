# predicting-the-selling-price-of-cars
This project consists in a supervised learning task and is about predicting the selling price of cars. The dataset is characterized by the following features:  
•	year: year of construction of the car   
•	km_driven: kilometers already driven by the car   
•	fuel: type of fuel of the car, part of [Diesel, Petrol, CNG, LPG]   
•	seller_type: type of seller, part of [Individual, Dealer, Trustmark Dealer]   
•	transmission: type of transmission of the car, part of [Manual, Automatic]   
•	owner: indication of the owner’s rank, part of [First Owner, Second Owner, Third Owner, Fourth & Above Owner, Test Drive Car]   
•	mileage: mileage of the car  
•	engine: CC of the engine of the car  
•	max_power: maximum power of the car   
•	torque: torque of the car   
•	seats: number of seats in the car   
Features are thus either quantitative or qualitative.   
  
Questions  
1.	Clean the data:  
a.	name: extract the car brand and make it a new feature     
b.	mileage & engine & max_power: keep only the numeric value and get rid of characters     
c.	torque: create 2 features, one with Nm values and one with rpm values. In case, they are 2 rpm values, calculate the average of these values.   
d.	Removing rows for which data is missing or dirty     
e.	Removing duplicated rows, if any   
   
2.	Build a linear regression model on your training set, and:   
a.	Using MSE, compare the training metric with the test metric and conclude about overfitting    
b.	Analyze the validity of the model, using a F-test at a p-value’s threshold of 5%   
c.	Analyze the coefficient’s significance, using a t-test at a p-value’s threshold of 5%. Exclude the features that should be excluded  so to build your final model   
d.	Repeat steps a-b-c for your final model   
e.	For your final model only, list the significant features and their coefficients   
f.	For your final model only, analyze the coefficient of the intercept, of one quantitative feature and one qualitative feature on the target feature, if any    
   
3.	Build an Elastic net model:   
a.	Based on cross-validation (5 folds), check for the best value of the l1-l2 allocation (𝜃) and quantity of regularization (𝜆) and create a model accordingly based on the error     
b.	Based on your final model, using MSE, compare the training metric with the test metric and conclude about overfitting   
c.	List the features kept in your model as well as their coefficients   
   
4.	Build a regression tree model on your training set , and:   
a.	Using MSE, compare the training metric with the test metric and conclude about overfitting   
b.	Mention the depth of your tree and the features involved in the splits   
c.	Based on cross-validation (5 folds), check for the best size of the tree and prune it accordingly   
d.	Repeat steps a-b on your pruned tree.    
e.	Conclude whether your pruned tree provides better results than the unpruned tree   
    
5.	Build a random forest model on your training set with the hyper-parameters [number of trees=10, number of features=sqrt], and:    
a.	Using MSE, compare the training metric with the test metric and conclude about overfitting   
b.	Obtain the feature importance of your model and comment it   
c.	Based on cross-validation (5 folds), check for the best number of trees  and model it accordingly   
d.	Repeat steps a-b on your optimized model.     
e.	Conclude whether your optimized model provides better results than the initial model    
   
6.	Based on all your models, which one do you consider the best and why?    
