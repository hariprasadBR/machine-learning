Machine Learning with Python
This repository contains Data Science projects in Python programming language completed by me for self-learning and demonstration purposes.

All the projects are done on Jupyter Notebooks (Notebook Server 5.6.0).

===============================================================================

### Libraries required
<B>The following libraries are required to successfully implement the projects.</B>

- Python 3.6+
- NumPy (for linear algebra)
- Pandas (for data preprocessing)
- Scikit-learn (for machine-learning)
- Matplotlib (for data visualization)
- Seaborn (for statistical data visualization)
- SciPy (for scientific computing)
- Statsmodels (statistical computation)


===============================================================================

The projects description are given in the readme document. The projects are divided into various categories listed below:-

Contents
## Supervised Learning : Regression Projects
- Simple Linear Regression Project: 
A Simple Linear Regression model to model the linear relationship between Sales and Advertising dataset .

- Multiple Linear Regression Project: 
In this project, I build a Multiple Linear Regression model to estimate the relative bike retal and housing price  dataset. I discuss the linear regression assumptions and various tools to estimate the model performance.

===============================================================================
Here's a brief summary of what you learnt in this session:

--> Machine learning models can be classified into the following two categories on the basis of the learning algorithm:
  1) Supervised learning method: Past data with labels is available to build the model.
    a) Regression: The output variable is continuous in nature.
    b) Classification: The output variable is categorical in nature.
  2) Unsupervised learning method: Past data with labels is not available.
    a) Clustering: There is no predefined notion of labels.
--> Past dataset is divided into two parts in the supervised learning method: 
  1) Training data is used for the model to learn during modelling.
  2) Testing data is used by the trained model for prediction and model evaluation.
--> Linear regression models can be classified into two types depending upon the number of independent variables: 
  a) Simple linear regression: This is used when the number of independent variables is 1.
  b) Multiple linear regression: This is used when the number of independent variables is more than 1.
--> The equation of the best fit regression line Y = β₀ + β₁X can be found by minimising the cost function (RSS in this case, using the ordinary least squares method), which is done using the following two methods:
  a) Differentiation
  b) Gradient descent 
--> The strength of a linear regression model is mainly explained by R², where R² = 1 - (RSS/TSS).
  a) RSS: Residual sum of squares
  b) TSS: Total sum of squares
--> RSE helps in measuring the lack of fit of a model on a given data. The closeness of the estimated regression coefficients to the true ones can be estimated using RSE. It is related to RSS by the formula: 
R
S
E
=
√
R
S
S
d
f
, where 
d
f
=
n
−
2
 and 
n
 is the number of data points.
## Supervised Learning : Classification Projects
- Logistic Regression Project: 
In this project, I train a binary Logistic Regression classifier to predict whether or not it will rain tomorrow in Australia. I have used Rain in Australia dataset from the Kaggle website. I have demonstrated feature engineering techniques alongwith Recursive Feature Elimination with Cross-validation, k-fold Cross Validation and GridSearch CV in this project.

- Support Vector Machines Project: 
In this project, I build a Support Vector Machines classifier to classify a Pulsar star. I have used the Predicting a Pulsar Star dataset from the Kaggle website. I have discussed the kernel trick in this project. I have used Stratified Cross-Validation technique alongwith GridSearch CV in this project.

- k Nearest Neighbours Project: 
k Nearest Neighbours is the simplest of all machine learning algorithms. In this project, I build a kNN classifier to classify the patients suffering from Breast Cancer. I have used the Breast Cancer Wisconsin (Original) Data Set from the UCI Machine Learning Repository.

- Naive Bayes Classification Project: 
In this project, I build a Naïve Bayes Classifier to classify a person's salary. I implement Naive Bayes Classification with Python and Scikit-Learn to predict whether a person makes over 50K a year. I have used Adult Data Set from the UCI Machine Learning Repository website.

- Decision Tree Classification Project: 
Classification and Regression Trees or CART are very popular machine learning algorithms. In this project, I build two Decision Tree Classifier models - with criterion gini and entropy to predict the safety of the car. I have used the Car Evaluation Data Set from the UCI Machine Learning Repository website.

- Random Forest Classification Project: 
In this project, I build two Random Forest Classifier models (with 10 and 100 decision-trees) to predict safety of the car. The accuracy increases with number of decision-trees. I have also demonstrated the feature selection process using the Random Forest model. I have used the Car Evaluation Data Set from the UCI Machine Learning Repository website.

- XGBoost Classification Project: 
XGBoost is an acronym for Extreme Gradient Boosting. In this project, I implement XGBoost with Python and Scikit-Learn to classify the customers from two different channels as Horeca (Hotel/Retail/Café) customers or Retail channel (nominal) customers. I have used Wholesale customers data set from UCI Machine learning repository.

===============================================================================

## Unsupervised Learning Projects
- K Means Clustering Project: 
K-Means clustering is used to find intrinsic groups within the unlabelled dataset and draw inferences. In this project, I implement K-Means clustering with Python and Scikit-Learn. I have used Facebook Live Sellers in Thailand dataset for this project from the UCI machine learning repository.


===============================================================================

Recommender Systems Project
Recommender Systems with Python: Recommender Systems are one of the most popular and widely used application of data science. In this project, I build a Recommender System with Python. I discuss various types of recommender systems including Content-based and Collaborative filtering recommender systems. Also, I discuss matrix factorization and how to evaluate recommender systems.


===============================================================================

## Statistical Analysis Projects
- Descriptive Statistics Project: Descriptive Statistics is the subject matter of this project. It gives us the basic summary measures about the dataset. The summary measures include measures of central tendency (mean, median and mode) and measures of variability (variance, standard deviation, minimum/maximum values, IQR (Interquartile Range), skewness and kurtosis).

- Inferential Statistics Project: Inferential Statistics is the process of drawing inferences about the population from the sample data. In this project, I have discussed various inferential statistical concepts and their practical applications. I have discussed Central Limit Theorem, t-test, ANOVA , Chi-square goodness of fit test and Correlation analysis.

- Hypothesis Testing Project: Hypothesis testing is a statistical tool to test an assumption regarding the population parameter. This project is dedicated towards hypothesis testing. In this project, I have discussed, hypothesis testing, p-value, significance level, types of errors in hypothesis testing and one-tailed and two-tailed tests.

===============================================================================

## Data Cleaning and Preprocessing Projects
- Data Cleaning with Python and Pandas: In this project, I discuss principles of tidy data and signs of an untidy data. I discuss EDA and present ways to deal with outliers and missing and negative numerical values. I discuss how to check for missing values with ASSERT statement. I present how to reshape data using the pandas melt() function.

- Data Preprocessing Project- Dealing with missing numerical values: This project describes various techniques to deal with missing numerical values. I have discussed how to drop missing values, fill missing values with test-statistic and imputer. I discuss how to check for missing values with ASSERT statement.

- Data Preprocessing Project- Dealing with text and categorical data: In this project, I discuss various Scikit-learn classes to deal with text and categorical data. The classes are LabelEncoder, OneHotEncoder, LabelBinarizer, DictVectorizer, CountVectorizer, TfidfVectorizer and TfidfTransformer. I also discuss tokenization and vectorization.

- Data Preprocessing Project-Feature Scaling: Feature Scaling is the process used to standardize range of independent variables so that they can be mapped onto same scale. In this project, I have discussed useful estimators related to Feature Scaling. The estimators are MinMaxScaler, StandardScaler, MaxAbsScaler, RobustScaler, Normalizer, Binarizer and scale.

- Data Preprocessing Project- Imbalanced Classes Problem: Imbalanced classes is a major problems in machine learning. In this project, I discuss imbalanced classes problem and the approaches to deal with this problem. I have used the Credit Card Fraud Detection dataset, downloaded from the Kaggle website.

===============================================================================

# Data Analysis Projects
- Exploratory Data Analysis with Python: This project is all about Exploratory Data Analysis. In this project, I explore the Absenteeism at work dataset. I discuss univariate and multivariate useful techniques to explore this dataset.

- Data Analysis with Pandas: Pandas is an open source library for data analysis in Python. In this project, I explore Pandas and important data analysis tools of pandas. I have used the BlackFriday dataset downloaded from Kaggle website.

- Data Analysis with NumPy: NumPy is the fundamental library of Python which is required for scientific computing. In this project, I explore NumPy and various data analysis tools of NumPy.

- Time Series Analysis with Python: A time series is a series of data points recorded at different time intervals. The time series analysis means analyzing the time series. In this project, I implement a Seasonal ARIMA time series model in Python to predict Occupancy rates of car parks in Parking Birmingham Data Set.

===============================================================================

## Data Visualization Projects
- Data Visualization with Matplotlib: Matplotlib is the basic data visualization library of Python. In this project, I describe Matplotlib, its object hierarchy, its interfaces, different plot types with Matplotlib and various customization techniques with Matplotlib.

- Data Visualization with Seaborn: Seaborn is a Python data visualization library based on Matplotlib. In this project, I explore Seaborn. I discuss Seaborn API overview, its functionality, setting Seaborn aesthetic parameters and colour palette. I discuss different distributions, various plot types and multi-plot grids with seaborn.
