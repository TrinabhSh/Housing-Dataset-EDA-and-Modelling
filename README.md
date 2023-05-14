# Boston-Housing-EDA-with-Modelling

In this project I have taken the famous Boston Housing Dataset and tried to do an EDA (Exploratory Data Analysis) to and visualise them. I've also fitted a multiple linear regressor that predicts the price of the houses.

[![alt text](https://camo.githubusercontent.com/613e5dd9c2a637e57bea0baa36b28144726ee4df54cc8bce314b108d24989264/68747470733a2f2f63646e31302e626f73746f6e6d6167617a696e652e636f6d2f77702d636f6e74656e742f75706c6f6164732f73697465732f322f323032322f30362f686f7573696e672d636f7374732d73746f72792e6a7067)](https://camo.githubusercontent.com/613e5dd9c2a637e57bea0baa36b28144726ee4df54cc8bce314b108d24989264/68747470733a2f2f63646e31302e626f73746f6e6d6167617a696e652e636f6d2f77702d636f6e74656e742f75706c6f6164732f73697465732f322f323032322f30362f686f7573696e672d636f7374732d73746f72792e6a7067)

## Exploratory Data Analysis and Multiple Linear Regression on Boston Housing Dataset

This dataset contains information about 506 census tracts of Boston from the 1970 census. As an aspiring data scientist, understanding how to model data like this is of great importance to me. In this kernel, I will use the Boston housing data by Harrison and Rubinfeld (1979) and explore which factors affect the median value of homes. I will perform a linear regression analysis on the same.

## Boston Housing Data

The data has following features, medv being the target (dependent) variable:

-   crim - per capita crime rate by town
    
-   zn - proportion of residential land zoned for lots over 25,000 sq.ft
    
-   indus - proportion of non-retail business acres per town
    
-   chas - Charles River dummy variable (= 1 if tract bounds river; 0 otherwise)
    
-   nox - nitric oxides concentration (parts per 10 million)
    
-   rm - average number of rooms per dwelling
    
-   age - proportion of owner-occupied units built prior to 1940
    
-   dis - weighted distances to five Boston employment centres
    
-   rad - index of accessibility to radial highways
    
-   tax - full-value property-tax rate per USD 10,000
    
-   ptratio - pupil-teacher ratio by town
    
-   black - proportion of blacks by town
    
-   lstat - percentage of lower status of the population
    
-   medv - median value of owner-occupied homes in USD 1000’s
    

## We will structure the code as follows

1.  Loading the data
    
2.  Preparing the data
    
3.  Exploratory Data Analysis
    
4.  Building the model and accuracy analysis
    
5.  Final Analysis of the model
    

## These are some of the insights

[![Insight Images - Free Download on Freepik](https://camo.githubusercontent.com/291a71b6d25013c8310c97650ecc9e9752fa0a232c199ac8beeef8db4a5d539d/68747470733a2f2f696d672e6672656570696b2e636f6d2f667265652d766563746f722f6772616469656e742d696e7369676874732d696c6c757374726174696f6e5f32332d323134393332323234312e6a70673f773d32303030)](https://camo.githubusercontent.com/291a71b6d25013c8310c97650ecc9e9752fa0a232c199ac8beeef8db4a5d539d/68747470733a2f2f696d672e6672656570696b2e636f6d2f667265652d766563746f722f6772616469656e742d696e7369676874732d696c6c757374726174696f6e5f32332d323134393332323234312e6a70673f773d32303030)

-   The median value of owner-occupied homes in the Boston suburbs ranges from $5,000 to $50,000, with a mean of $22,533.
-   The distribution of the median value of homes is slightly right-skewed, with a few suburbs having very high median home values (up to $50,000).
-   The variables that have the strongest positive correlation with the median value of homes are the average number of rooms per dwelling and the proportion of residential land zoned for lots over 25,000 square feet.
-   The crime rate per capita variable has a skewed distribution, with a few suburbs having a very high crime rate compared to others.
-   The Charles River dummy variable (which indicates whether a suburb borders the river or not) has a significant impact on the median value of homes, with suburbs that border the river tending to have higher median home values.
-   There are both positive and negative correlation with the response varaible. Crim, indus, nox, age, rad, tax, ptratio, lstat all of them have a negative correlation with the lstat one having the strongest correlation. While, zn, chas, rm, dis and black have a positive correlation with rm having the strongest positive correlation. rad and tax have a strong positive correlation of 0.91 which implies that as accessibility of radial highways increases, the full value property-tax rate per $10,000 also increases. indus has a strong positive correlation with nox indicating that the concentration of nitrogen oxides are very high in industrial areas.
-   We can see a strong positive correlation between distance of 5 employment center from town and price. The closer/farther the employment center from town the more/less the housing prices.
-   We can see a strong negative correlation between NOX concentration in air and price. The more/less concentration of NOX is in air the less/more the housing prices.

## Multiple Linear Regression

[![Linear_regression_intro.gif](https://github.com/Infinity1008/Concept_explainers/raw/main/Regression/Linear_regression/animated_gifs/Linear_regression_intro.gif?raw=true)](https://github.com/Infinity1008/Concept_explainers/blob/main/Regression/Linear_regression/animated_gifs/Linear_regression_intro.gif?raw=true)  I have also fitted a Multiple Linear Regression model which predicts the price of the house, feel free to look at the  `ipnyb`  file to explore more.

## FIN.
