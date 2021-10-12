# Linear regression

## library used 
- numpy
- pandas
- matplotlib
- seaborn
- statsmodel
- sklearn


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

#### 7) Underfitting and Overfitting
When we fit a model, we try to find the optimised, best-fit line, which can describe the impact of the change in the independent variable on the change in the dependent variable by keeping the error term minimum. While fitting the model, there can be 2 events which will lead to the bad performance of the model. These events are

Underfitting 
Overfitting
Underfitting 
Underfitting is the condition where the model could not fit the data well enough. The under-fitted model leads to low accuracy of the model. Therefore, the model is unable to capture the relationship, trend or pattern in the training data. Underfitting of the model could be avoided by using more data, or by optimising the parameters of the model.

Overfitting
Overfitting is the opposite case of underfitting, i.e., when the model predicts very well on training data and is not able to predict well on test data or validation data. The main reason for overfitting could be that the model is memorising the training data and is unable to generalise it on test/unseen dataset. Overfitting can be reduced by doing feature selection or by using regularisation techniques. 



#### 8) There are 2 types of linear regression:
1. Simple Linear Regression
2. Multiple Linear Regression


#### Error Terms or Residuals (ϵ):
It is the difference between the actual and the predicted data point in the x-y coordinate graph
Objective of Linear Regression:
The goal of linear regression is to perform predictive analytics and it is done by making the machine learn the science of generating a trained (best fitted) line that will very well generalize how new and unknown data (test set or new dataset) will be evaluated, and how the fitted line will be able to accurately estimate new or unknown datasets.


# Steps to be followed in Linear Regression Algorithm:
1. Reading and understanding the data
a. Importing required libraries like pandas & numpy for data analysis and manipulation and seaborn & matplotlib for data visualization
b. Cleaning and manipulating data to make it up to the standards that exploratory data analysis can be performed by treating null values if any, updating to necessary formats, changing data types if needed, removing unwanted rows or columns etc. The raw data in whatever condition you get must be squeaky cleaned of any muck before assessing it for visualization.
2. Visualizing the data (Exploratory Data Analysis)
a. Visualizing numerical variables using scatter or pairplots in order to interpret business /domain inferences.
b. Visualizing categorical variables using barplots or boxplots in order to interpret business/domain inferences.
3. Data Preparation
a. Converting categorical variables with varying degrees of levels into dummy variables (numerical in nature) so that these variables can be represented during model building in order to contribute to the best fitted line for the purpose of better prediction.
4. Splitting the data into training and test sets
a. Splitting the data into two sections in order to train a subset of dataset to generate a trained (fitted) line that will very well generalize how new and unknown data (test set or new dataset) will be evaluated, and how the fitted line will be able to accurately estimate new or unknown datasets. Generally, the train-test split ratio is 70:30 or 80:20.
b. Rescaling the trained model: It is a method used to normalize the range of numerical variables with varying degrees of magnitude. For e.g. height or bmi or age are of different magnitude and units or some feature may have values in 10000s while feature may contain values in the magnitude of 10s or 100s, then the contribution of each feature for the dependent variable will be different
5. Building a linear model
a. Forward Selection: We start with null model and add variables one by one. These variables are selection on the basis of high correlation with target variable. First we select the one, which has highest correlation and then we move on to the second highest and so on.
b. Backward Selection: We add all the variables at once and then eliminate variables based on high multicollinearity (VIF>5) or insignificance (high p- values).
c. RFE or Recursive Feature Elimination is more like an automated version of feature selection technique where we select that we need “m” variables out of “n” variables and then machine provides a list of features with importance level given in terms of rankings. A rank 1 means that feature is important for the model, while a rank 4 implies that we are better off, if we don’t consider the feature.
6. Residual analysis of the train data:
a. It tells us how much the errors (y_actual — y_pred) are distributed across the model. A good residual analysis will signify that the mean is centred around 0.
![1_TC5gcBCtVg5w-OqSA85A7g](https://user-images.githubusercontent.com/84274712/136905211-9ecccaa8-577e-426a-92f3-3258db451008.png)

The residual errors are centered around 0
7. Making predictions using the final model and evaluation:
a. We will predict the test dataset by transforming it onto the trained dataset
b. Divide the test sets into X_test and y_test and calculate r2_score of test set. The train and test set should have similar r2_score. A difference of 2–3% between r2_score of train and test score is acceptable as per the standards.

Feature Scaling is a technique to standardize the independent features present in the data in a fixed range. It is performed during the data pre-processing to handle highly varying magnitudes or values or units. If feature scaling is not done, then a machine learning algorithm tends to weigh greater values, higher and consider smaller values as the lower values, regardless of the unit of the values.
![Capture](https://user-images.githubusercontent.com/84274712/136905556-a10f0417-14a0-424f-a993-e8d7b2cea027.PNG)


