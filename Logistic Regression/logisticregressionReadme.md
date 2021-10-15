Summary
In this session, you learnt how to build a multivariate logistic regression model in Python. The equation for multivariate logistic regression is basically just an extension of the univariate equation:

 

P
=
1
1
+
e
−
(
β
0
+
β
1
X
1
+
β
2
X
2
+
β
3
X
3
+
.
.
.
+
β
n
X
n
)

 

The example used for building the multivariate model in Python was the telecom churn example. Basically, you learnt how Python can be used to decide the probability of a customer churning based on the value of 21 predictor variables such as monthly charges, paperless billing, etc.

 

First, the data was imported, which was present in 3 separate csv files. After creating a merged master data set, one that contains all 21 variables, data preparation was done, which involved the following steps:

Missing value imputation

Outlier treatment

Dummy variable creation for categorical variables

Test-train split of the data

Standardisation of the scales of continuous variables

 

After all of this was done, a logistic regression model was built in Python using the function GLM() under statsmodel library. This model contained all the variables, some of which had insignificant coefficients. Hence, some of these variables were removed first based on an automated approach, i.e. RFE and then a manual approach based on VIF and p-value.

 

Apart from this, you also learnt about confusion matrix and accuracy and saw how accuracy was calculated for a logistic regression model.
