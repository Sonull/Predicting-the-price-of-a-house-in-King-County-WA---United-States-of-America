# Information about the Analysis
* The dataset contains selling price for homes sold in King County between May 2014 and May 2015 
* Total number of variables = 19 (excluding ‘price’ and ‘id’)
* Total number of observations = 21,613
* Source of data : www.kaggle.com
* The level of significance, alpha is taken to be 0.05 for the analysis

# Goal of the Anaysis
Build a multiple linear regression model to predict the selling price of a house in King County, United States of America

# Dependent Variable
The variable ‘price’ is the dependent variable. In the dataset, it is the amount at which the house was sold.

# Independent Variables
* The following numeric variables have been considered as independent variables for the regression analysis:
  * bedrooms		   : 	Number of bedrooms in each house					
  * bathrooms		   :	Number of bathrooms in each house
  * sqft_living		 :	Square footage of the house
  * sqft_lot		   :	Square footage of the lot
  * floors		     :	Total number of floors in the house
  
# Visualization of the data
![chart1](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/chart1.png)

![graph1](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/graph1.png)

* The distribution of number of bedrooms for these 21,613 houses follows a normal distribution which is positively skewed
* There are maximum number of houses with 3 bedrooms followed by houses with 4 bedrooms

![chart2](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/chart2.png)

![graph2](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/graph2.png)

* There are maximum number of houses with 2.5 bathrooms followed by houses with 1 bathroom
* The highest number of bathrooms in a house is 8
* 87% of the houses have less than or equal to 2.75 bathrooms

