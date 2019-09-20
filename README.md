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

# Chart 1
![chart1](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/chart1.png)

![graph1](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/graph1.png)

* The distribution of number of bedrooms for these 21,613 houses follows a normal distribution which is positively skewed
* There are maximum number of houses with 3 bedrooms followed by houses with 4 bedrooms

# Chart 2
![chart2](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/chart2.png)

![graph2](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/graph2.png)

* There are maximum number of houses with 2.5 bathrooms followed by houses with 1 bathroom
* The highest number of bathrooms in a house is 8
* 87% of the houses have less than or equal to 2.75 bathrooms

# Chart 3
![chart3](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/chart3.png)

![graph3](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/graph3.png)
* There are a lot of outliers in the variable ’sqft_living’ which provides the information around the square footage of each house
* About 50% of the houses have square footage of <= 2000 sqft.
* 25% of the houses have square footage of <= 1400 sqft approx. while 75% of the houses have square footage less than 2500 sqft approx

# Chart 4
![chart4](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/chart4.png)

![graph4](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/graph4.png)
* The oldest houses were built in 1900
* The construction of houses has increased over time
* Highest number of houses sold were built between 2000-2010 so, they were about 5 years old at the time of sale
* There were about 1000 houses which were at least a decade or more old when sold 

# Correlation between the dependent variable and all independent variables

# Hypothesis Testing
* Ho : Population Correlation Coefficient is 0
* H1 : Population Correlation Coefficient is not 0
* Rejection Criteria
  * If p value < alpha, we reject Ho 

# Correlation between 'price' and 'bedrooms'
![Scatter1](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/Scatter1.png)

![scatter1](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/scatter1.png)

* The scatterplot shows that there exists a moderately strong positive linear relationship between the square footage of the house and the price

![corr1](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/corr1.png)
* The correlation coefficient between ‘bedrooms’ and ‘price’ = 0.3083496
* p-value=0
* Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the correlation coefficient is significant. That is, there is evidence to suggest that there is significant positive correlation between the number of bedrooms and the price of the house at 5% level of significance

# Correlation between 'price' and 'bathrooms'
![Scatter2](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/Scatter2.png)

![scatter2](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/scatter2.png)

* The scatterplot shows that there is a weak positive linear relationship between the square footage of the lot and the price of the house

![corr1](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/corr1.png)
* The correlation coefficient between ‘bathrooms’ and ‘price’ = 0.5251375
* p-value=0
* Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the correlation coefficient is significant. That is, there is there is evidence to suggest that there is significant positive correlation between the number of bathrooms and the price of the house at 5% level of significance

