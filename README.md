# SC1015-Group-10-Project

## About 

This is a Mini-Project for SC1015 (Intro To Data Science and Artificial Intelligence) which uses the datasets from World Bank and Global Health Data Exchange to analyse how Health-Adjusted Life Expectancy (HALE) and Life Expectancy can be affected by different predictors and to find a set of predictors that can be used to maximize HALE. 
For walkthrough, view the source code in order from: 

1. [Data Preparation and Cleaning](https://github.com/Sherylleong/SC1015-Group-10-Project/blob/main/Data%20Preparation%20and%20Cleaning.ipynb)
    - iniital data exploration to prepare for cleaning
    - extraction, preparation and cleaning of data

2. [Data Visualisation and Analysis](https://github.com/Sherylleong/SC1015-Group-10-Project/blob/main/Data%20Visualization%20and%20Analysis.ipynb)
    - visualisation of differences in trends and distribution between life expectancy and HALE
    - exploratory analysis and visualisation of all features over time
    - visualisation and analysis of relationships between all metrics against HALE
    - 
3. [Machine Learning](https://github.com/Sherylleong/SC1015-Group-10-Project/blob/main/Machine%20Learning.ipynb)
    - training and evaluation of linear regression, regression tree and random forest models to predict HALE
    - analysis of coefficients and importances of various features in different models
    
## Contributors
- Leong Kit Ye @Sherylleong
- Khant Zayar @KZY201101
- Bruce Li Luyun @


## Problem Definition 
- Can we predict the Life Expectancy and Health-Adjusted Life Expectancy(HALE) of a country based on other data such as its population, GDP etc?
- Which set of data are the most useful in predicting the HALE and Life Expectancy? 
- Which model would provide the most accurate results?



###  Datasets used  ###
Global Health Data Exchange (GHDx) datasets (https://ghdx.healthdata.org/):
1. **hale.csv** : Health-Adjusted Lide Expectancy (HALE) of all countries and territories from years 2000-2019.
    
World Bank datasets (https://data.worldbank.org/):    
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
