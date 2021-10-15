
build a multivariate logistic regression model in Python. The equation for multivariate logistic regression is basically just an extension of the univariate equation:
![eq](https://user-images.githubusercontent.com/84274712/137467507-04e25cec-1cee-4f99-8fea-6aed42f4fa4b.PNG)


 

The example used for building the multivariate model in Python was the telecom churn example. Basically, learnt how Python can be used to decide the probability of a customer churning based on the value of 21 predictor variables such as monthly charges, paperless billing, etc.

 

- First, the data was imported, which was present in 3 separate csv files. After creating a merged master data set, one that contains all 21 variables, data preparation was done, which involved the following steps:

- Missing value imputation

- Outlier treatment

- Dummy variable creation for categorical variables

- Test-train split of the data

- Standardisation of the scales of continuous variables

 

After all of this was done, a logistic regression model was built in Python using the function GLM() under statsmodel library. This model contained all the variables, some of which had insignificant coefficients. Hence, some of these variables were removed first based on an automated approach, i.e. RFE and then a manual approach based on VIF and p-value.

 

Apart from this, t confusion matrix and accuracy and saw how accuracy was calculated for a logistic regression model.

So to summarise, the steps that you performed throughout the model building and model evaluation were:
    
1) Data cleaning and preparation
    a) Combining three dataframe    
    b) Handling categorical variables
        A) Mapping categorical variables to integers
        B) Dummy variable creation       
    c) Handling missing values    
2) Test-train split and scaling
3) Model Building
    a) Feature elimination based on correlations
    b) Feature selection using RFE (Coarse Tuning)
    c) Manual feature elimination (using p-values and VIFs)    
4) Model Evaluation
    1) Accuracy
    2) Sensitivity and Specificity
    3) Optimal cut-off using ROC curve
    4) Precision and Recall   
5) Predictions on the test set
    
    
So first, classes were assigned to all the customers in the test data set. For this, a probability cutoff of 0.5 was used. The model thus made, was very accurate (Accuracy = ~80%), but it had a very low sensitivity (~53%). Thus, a different cutoff was tried out, i.e. 0.3, which resulted in a model with slightly lower accuracy (~77%), but a much better sensitivity (~78%). Hence, you learnt that you should not just blindly use 0.5 as the cutoff for probability every time you make a model. Business understanding must be applied. Here, that means playing around with the cutoff, until you get the most useful model.

 

Also, recall that the sensitivity of a model is the proportion of yeses (or positives) correctly predicted by it as yeses (or positives). Also, the specificity is equal to the proportion of nos (or negatives) correctly predicted by the model as nos (or negatives). For any given model, if the sensitivity increases by changing the cutoff, its specificity goes down.
High values of both cannot be achieved in a single model. Hence, you have to choose which one you would want to be higher. The safest option, though, is the one in which you just take the cutoff that equalises accuracy, sensitivity and specificity. But it totally depends on the business context. Sometimes you might want a higher sensitivity, sometimes you might want a higher specificity.

 

You also saw another view of things which was the Precision and Recall view. Those were very much related to sensitivity and specificity. Precision essentially means of the 'Yeses' predicted, how many were actually yeses. Recall on the other hand is that same as sensitivity, i.e. out of the total actual yeses, how many did you correctly predict.
