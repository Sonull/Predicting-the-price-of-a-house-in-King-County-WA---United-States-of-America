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

![corr2](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/corr2.png)
* The correlation coefficient between ‘bathrooms’ and ‘price’ = 0.5251375
* p-value=0
* Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the correlation coefficient is significant. That is, there is there is evidence to suggest that there is significant positive correlation between the number of bathrooms and the price of the house at 5% level of significance

# Correlation between 'price' and 'sqft_lot'
![Scatter3](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/Scatter3.png)

![scatter3](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/scatter3.png)

* The scatterplot shows that there is a mild positive linear relationship between the number of bedrooms of the house and the price of the house


![corr3](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/corr3.png)
* The correlation coefficient between ‘sqft_lot’ and ‘price’ = 0.08966086
* p-value=7.972505*10^(-40)
* Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the correlation coefficient is significant. That is, there is evidence to suggest that there is significant positive correlation between the square footage of the lot and the price of the house at 5% level of significance

# Correlation between 'price' and 'floors'
![Scatter4](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/Scatter4.png)

![scatter4](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/scatter4.png)

* The scatterplot shows that there is a moderate positive linear relationship between the number of bathrooms of the house and the price


![corr4](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/corr4.png)
* The correlation coefficient between ‘floors’ and ‘price’ = 0.2567939
* p-value=1.58101*10^(-322)
* Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the correlation coefficient is significant. That is, there is evidence to suggest that there is significant positive correlation between the number of floors and the price of the house at 5% level of significance

# Correlation between 'price' and 'sqft_living'
![Scatter5](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/Scatter5.png)

![scatter5](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/scatter5.png)

* The scatterplot shows that there is a mild positive linear relationship between the number of floors of the house and the price


![corr5](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/corr5.png)
* The correlation coefficient between ‘sqft_living’ and ‘price’ = 0.7020351
* p-value=0
* Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the correlation coefficient is significant. That is, there is evidence to suggest that  there is significant positive correlation between the square footage of the house and the price of the house at 5% level of significance

# Multivariate Linear Regression Analysis

# Iteration 1
![model1code](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/model1code.png)

![model1results](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/model1results.png)

* Rsquare = 0.5087 implies that 50% of the variation in the dependent variable is explained by the independent variables
* F test:
  * Ho: Beta1 = Beta2=Beta3=….Betan=0 i.e all Beta coefficients are 0
  * H1: At least one of the regression coefficients is not equal to 0
  * Since, p-value of F statistic is < 2.2e-16 (and therefore, less than alpha), we reject the Ho and conclude that that at least one of the predictor variables in our model has a significant relationship with our outcome variable

# Test of significance of each variable
* Ho : Beta is 0 
* H1 : Beta is not 0
* Rejection Criteria
  * If p value < alpha, we reject Ho

* ‘bedrooms’ :
  * Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the coefficient is significant. Thus, the variable ‘bedrooms’ is statistically significant
* ‘bathrooms’ :
  * Since p-value > alpha (0.05), we fail to reject the null hypothesis and conclude that the coefficient is insignificant. Thus, the variable ‘bathrooms’ is statistically insignificant
* ‘sqft_living’:
  * Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the coefficient is significant. Thus, the variable ‘sqft_living’ is statistically significant
* ‘sqft_lot’:
  * Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the coefficient is significant. Thus, the variable ‘sqft_lot’ is statistically significant
* ‘floors’:
  * Since p-value > alpha (0.05), we fail to reject the null hypothesis and conclude that the coefficient is insignificant. Thus, the variable ‘floors’ is statistically insignificant
  
# Re-running the model after dropping the insignificant variables

# Iteration 2
![model2code](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Codes/model2code.png)

![model2results](https://github.com/Sonull/Price-Prediction-using-Multiple-Linear-Regression/blob/master/Visualization/model2results.png)

* Rsquare = 0.5086 implies that 50% of the variation in the dependent variable is explained by the independent variables
* F test:
  * Ho: Beta1 = Beta2=Beta3=….Betan=0 i.e all Beta coefficients are 0
  * H1: At least one of the regression coefficients is not equal to 0
  * Since, p-value of F statistic is < 2.2e-16, we reject the Ho and conclude that that at least one of the predictor variables in our model has a significant relationship with our outcome variable

# Test of significance of each variable
* Ho : Beta is 0 
* H1 : Beta is not 0
* Rejection Criteria
  * If p value < alpha, we reject Ho

* ‘bedrooms’ :
  * Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the coefficient is significant. Thus, the variable ‘bedrooms’ is statistically significant
* ‘sqft_living’:
  * Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the coefficient is significant. Thus, the variable ‘sqft_living’ is statistically significant
* ‘sqft_lot’:
  * Since p-value < alpha (0.05), we reject the null hypothesis and conclude that the coefficient is significant. Thus, the variable ‘sqft_lot’ is statistically significant

# Conclusion
* Thus, the equation of multiple linear regression model is:

## Price of the house = 82780 – 58800 * bedrooms + 317.9 * sqft_living – 0.3818 * sqft_lot

 * An increase of 1 bedroom will decrease the price of the house by $58,800 when all other variables are held constant
 * An increase in the square footage of the house by 1sqft will increase the price of the house by $317.9 when all other variables are held constant
 * An increase in the square footage of the lot by 1sqft will decrease the price of the house by $0.3818 when all other variables are held constant

