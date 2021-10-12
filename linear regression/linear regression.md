# Linear regression
#### 1) What is Regression?

Regression is a method of modeling a target value based on independent predictors. It is a statistical tool which is used to find out the relationship between the outcome variable also known as the dependent variable, and one or more variable often called as independent variables.  This method is mostly used for forecasting and finding out cause-and-effect relationships between variables. Regression techniques mostly differ based on the number of independent variables and the type of relationship between the independent and dependent variables.

#### 2) When and why do you use Regression?

Regression is performed when the dependent variable is of continuous data type and Predictors or independent variables could be of any data type like continuous, nominal/categorical etc. Regression method tries to find the best fit line which shows the relationship between the dependent variable and predictors with least error. 
In regression, the output/dependent variable is the function of an independent variable and the coefficient and the error term.

#### 3) What is Linear Regression?

Linear regression strives to show the relationship between two variables by applying a linear equation to observed data.The measure of the extent of the relationship between two variables is shown by the correlation coefficient. The range of this coefficient lies between -1 to +1. This coefficient shows the strength of the association of the observed data for two variables.


#### 4) The equation for the best-fit line:

A linear regression line equation is written in the form of:

Y = a + bX

where X is the independent variable and plotted along the x-axis

Y is the dependent variable and plotted along the y-axis

The slope of the line is b, and a is the intercept (the value of y when x = 0).

Through the best fit line, we can describe the impact of change in independent variables on the dependent variable. 


There are four assumptions associated with a linear regression model:

a) Linearity: The relationship between independent variables and the mean of the dependent variable is linear. 
b) Homoscedasticity: The variance of residuals should be equal.
c) Independence: Observations are independent of each other.
d) Normality: For any fixed value of an independent variable, the dependent variable is normally distributed.

#### 5) Isn’t Linear Regression from Statistics?

Isn’t it a technique from statistics? Machine learning, more specifically the field of predictive modelling is primarily concerned with minimizing the error of a model or making the most accurate predictions possible, at the expense of explainability. In applied machine learning, we will borrow and reuse algorithms from many different fields, including statistics and use them towards these ends.


#### 6) Performance of Regression?

The performance of the regression model can be evaluated by using various metrics like 
- MAE
- MAPE
- RMSE
- R-squared 
- adjusted r-square etc

- Mean Absolute Error (MAE)
By using MAE, we calculate the average absolute difference between the actual values and the predicted values. 

- Mean Absolute Percentage Error (MAPE) 
MAPE is defined as the average of the absolute deviation of the predicted value from the actual value. It is the average of the ratio of the absolute difference between actual & predicted values, and actual value. 

- Root Mean Square Error (RMSE)
RMSE calculates the square root average of the sum of the squared difference between the actual and the predicted values.

- R-squared values
R-square value depicts the percentage of the variation in the dependent variable explained by the independent variable in the model.
R2 value ranges from 0 to 1. Higher the R-square value better the model. The value of R2 increases if we add more variables to the model irrespective of the variable contributing to the model or not. This is the disadvantage of using R2.
Specifically, this linear regression is used to determine how well a line fits’ to a data set of observations, especially when comparing models. Also, it is the fraction of the total variation in y that is captured by a model. Or, how well does a line follow the variations within a set of data.
![r-squared](https://user-images.githubusercontent.com/84274712/136902571-8144a6db-61f0-4ff0-8622-e4ef319cac9f.jpg)

R-Squared R2
![r-square-formula-1](https://user-images.githubusercontent.com/84274712/136903215-591cdf33-9c33-4485-a11f-1d1bbf463558.jpg)


- RSS = Residual sum of squares: It is the measure of the difference between the expected and the actual output. A small RSS indicates a tight fit of the model to the data. It is also defined as follows: 

- TSS = Total sum of squares: It is the sum of errors of the data points from the mean of the response variable. 

- Adjusted R-squared values
The disadvantage of R2 is fixed by the Adjust
ed R2 value. Adjusted R2 value will improve only if the added variable is making a significant contribution to the model. Adjusted R2 value adds penalty in the model.

where R2 is R-square value, n = total number of observations, and k = total number of variables used in the model. If we increase the number of variables, the denominator becomes smaller and the overall ratio will be high. Subtracting from 1 will reduce the overall Adjusted R2. So to increase the Adjusted R2, the contribution of additive features to the model should be significantly high.




