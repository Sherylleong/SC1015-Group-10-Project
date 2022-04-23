# SC1015-Group-10-Project

## About 

This is a Mini-Project for SC1015 (Intro To Data Science and Artificial Intelligence) which uses the datasets from World Bank and Global Health Data Exchange to analyse how Health-Adjusted Life Expectancy (HALE) and Life Expectancy (LE) can be affected by different predictors and to find a set of predictors that can be used to maximize HALE. 
For walkthrough, view the source code in order from: 

1. [Data Preparation and Cleaning](https://github.com/Sherylleong/SC1015-Group-10-Project/blob/main/Data%20Preparation%20and%20Cleaning.ipynb)
    - initial data exploration to prepare for cleaning
    - extraction, preparation and cleaning of data

2. [Data Visualisation and Analysis](https://github.com/Sherylleong/SC1015-Group-10-Project/blob/main/Data%20Visualization%20and%20Analysis.ipynb)
    - visualisation of differences in trends and distribution between LE and HALE
    - exploratory analysis and visualisation of all features over time
    - visualisation and analysis of relationships between all metrics against HALE
     
3. [Machine Learning](https://github.com/Sherylleong/SC1015-Group-10-Project/blob/main/Machine%20Learning.ipynb)
    - training and evaluation of linear regression, regression tree and random forest models to predict HALE and LE
    - analysis of coefficients and importances of various features in different models
    
## Contributors
- Leong Kit Ye @Sherylleong
- Khant Zayar @KZY201101
- Bruce Li Luyun @BruceLee7


## Problem Definition 
- Can we predict the Life Expectancy(LE) and Health-Adjusted Life Expectancy(HALE) of a country based on other data such as its population, GDP etc?
- Which set of data are the most useful in predicting the HALE and Life Expectancy? 
- Which model would provide the most accurate results?

## Models Used 
1. Multivariate Linear Regression 
2. Regression Trees
3. Random Forest Regression 

## What we learned from this project
- Handling multiple datasets with different formats and standardizing them 
- Merging multiple dataframes into a single dataframe with a convenient format for analysis
- Linear Regression from sklearn.linear_model 
- Regression Trees from sklearn.tree
- Random Forest Regression from sklearn.ensemble 
- Collaborating using Google Colab notebooks and Github
- Concept about feature importances 

## Conclusion 
Unsurprisingly, out of all the models, random forest tree regression is the most effective both in terms of R^2 score and RMSE in predicting HALE and LE. 
Analysing the models and results, it seems that HALE has a slightly more linear relationship with the predictors while life expectancy has a slighty more non-linear relationship with them, however, a sufficiently robust model such as random forest tree regression is still able to capture these relationships. 

From our visualizations, there is a clear correlation between response variables HALE/LE and some predictors such as the percentage of people using at least basic sanitation services, and GDP. This makes sense because having a high GDP and a large percentage of people being able to use basic sanitation services indicates that the country is at least developed to some degree and hence can provide better living standards. Having better living standards could mean that average HALE and LE could be higher.These observations proved to be consistent with the feature importances as shown by models as both access to basic sanitation services and GDP per capita are the most important metrics across all the models Thus, governments seeking to increase HALE can prioritise increasing these two metrics. 

It can also be seen that current health expenditure brings significant benefits to HALE and domestic private health expenditure has negligible impact on HALE, implying that government expenditure in the healthcare sector is what causes HALE to rise. Furthermore, while both age dependency ratio and population density have a negative impact on both HALE and life expectancy, age dependency ratio affects life expectancy more while population density affects HALE more. 

Given limited resources, our model can inform which areas countries can shift their limited resources in order to increase HALE and LE to ensure everyone lives long, healthy lives.

##  Datasets used  

### Global Health Data Exchange (GHDx) datasets (https://ghdx.healthdata.org/):
1. **hale.csv** : Health-Adjusted Lide Expectancy (HALE) of all countries and territories from years 2000-2019.
    
### World Bank datasets (https://data.worldbank.org/):    
1. **% basic sanitation services.csv** : Percentage of population with access to basic sanitation services of all countries from years 2000-2019.
2. **age dependency ratio.csv** : Age-dependency ratio (ratio of number of dependents e.g. children and elderly to number of workers) as percentage of working-age population of all countries from years 2000-2019.
3. **c02 emissions mtpc.csv** : CO2 emissions (metric tons per capita) of all countries from years 2000-2019.
4. **domestic private health expenditure.csv** : Domestic private health expenditure as a percentage of current health expenditure of all countries from years 2000-2019.
5. **gdppc.csv** : Gross Domestic Product (GDP) per capita of all countries from years 2000-2019.
6. **health expenditure %gdp.csv** : Health expenditure as a percentage of GDP of all countries from years 2000-2019.
7. **immunisation measles.csv** : Percentage of children aged 12-23 months who received measles vaccination for all countries from years 2000-2019.
8. **life expectancy.csv** : Average life expectancy of all countries from years 2000-2019.
9. **population density.csv** : Population desity of all countries from years 2000-2019.
10. **population.csv** : Population of all countries from years 2000-2019.
