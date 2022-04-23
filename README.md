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
The random forest model was the best at predicting life expectancy and HALE out of all the 3 models. It seems that both life expectancy and HALE had slightly nonlinear relationships with the data, but a sufficiently robust model such as random forest is able to capture these relationships. It seems that overall, the metrics chosen were able to btter predict life expectancy than HALE, but they can still predict HALE with high accuracy.

While using a robust model makes explanation of exactly how a metric affects HALE more difficult to explain, we can see that both access to basic sanitation services and GDP per capita are the most important metrics across all the models, as well as having positive correlations with HALE. Thus, governments seeking to increase HALE can prioritise increasing the two metrics. However, we must also keep in mind that correlation does not imply causation. For example, population density had a positive correlation with HALE, but logically a high population density would put a strain on current healthcare services. Instead, this could be explained by areas with high population densities also tending to be centres of economic activity, with richer citizens.

It can also be seen that current health expenditure brings significant benefits to HALE, but domestic private health expenditure has negligible impact on HALE, implying that government expenditure in the healthcare sector is what causes HALE to rise. Furthermore, age dependency ratio has a higher influence on life expectancy while current health expenditure has a higher influence on HALE. Thus a government seeking to improve HALE over life expectancy can know to prioritise health expenditure before addressing the issue of reducing age dependency ratio.

Given limited resources, our model can inform which areas countries can shift their limited resources in order to increase HALE to ensure everyone lives long, healthy lives.

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
