# simple linear regression
We consider the modelling between the dependent and one independent variable. When there is only one 
independent variable in the linear regression model, the model is generally termed as a simple linear 
regression model.

## Our Advertising Dataset
The Advertising data set we are going to use is from “An Introduction to Statistical Learning”, textbook by Gareth James, Robert Tibshirani, and Trevor Hastie, which consists of the sales of a product in 200 different markets, along with advertising budgets for the product in each of those markets for three different media: TV, radio, and newspaper.

## Our Objetive
- By training an inference model, a series of mathematical expressions we want to apply to our data that depends on a series of parameters. The values of parameters change through training in order for the model to learn and adjust its output.

The training loop consists in the following steps:
- First, we need to initialize the model parameters to some random values.
- Second, we need to read the training data -for each example, and possibly using randomization strategies in order to assure that training is stochastic.
- Third, we need to execute the inference model on the training data, getting for each training example the model output with the parameter values.
- Four, we compute the loss.
- And last, we adjuts the model parameters.
We need to repeat this process several times, according to the learning rate. After the training of the model is done we need to apply an evaluation phase.
