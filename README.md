# Project 1: World Development Statistics

### Problem Statement

Smoking is a very prevalent problem in various countries and regions across the world. Smoking can be the source of serious health problems and can ultimately lead to death in many cases. With products such as cigarettes and vapes becoming more and more popular as time goes on, there is a high chance that there will be an increase in the amount of deaths throughout various countries. The objective of this project is to find whether countries with a low life expectancy also have a high rate of smoking in the year 2020.


### Data Dictionary

|**country**|object|population.csv|The name of the country being studied 

|**code**|object|share-of-adults-who-smoke.csv|Country code for specific country

|**tabacco_use**|float|share-of-adults-who-smoke.csv|The percent of adults who smoke in the respective country

|**year**|int|share-of-adults-who-smoke.csv|Year the data was taken from

|**1800_pop**|object|merged_data.csv|Population in the country in the given years

|**1800_life**|object|merged_data.csv|Life expectancy in the country in the given years


### Executive Summary

####  Datasets

As smoking cigarettes has become more and more relevant throughout the years, there are also a number of health problems that arise with it. While the public is aware that smoking can lead to serious conditions such as lung cancer, it is still unknown whether there is a high correlation between the two variables. This project aims to find whether there is a relation between tabacco usage and life expectancy in various countries in the year 2020.

This project used three data sources: 
1) population.csv (Population by Country) 
2) life_expectancy.csv (Life Expectancy by Country)
3) share-of-adults-who-smoke.csv (Tabacco Usage by Country)

#### Data Cleaning

To begin, the data was cleaned thoroughly. This included changing all the column names to lower case and using an underscore instead of spaces where necessary, dropping unwanted missing values, changing any problematic datatypes, and applying custom functions where needed (eg. convert function applied to population.csv dataframe). After the cleaning was performed, all three datasets were merged together to form merged_df.csv. This merged file was used to execute Exploratory Data Analysis and a number of questions were asked to find relationships and dig deeper into the problem:

#### Exploratory Data Analysis

1) Which countries have the highest and lowest tabacco use for 2020?
2) Which countries have the highest and lowest life expectancy for 2020?
3) Which country had the biggest difference in population size comparing 1800 to 2020?
4) Which country had the lowest difference in population size comparing 1800 to 2020?
5) Which country had the biggest change in life expectancy comparing 1800 to 2020?
6) Which country had the smallest change in life expectancy comparing 1800 to 2020?

To answer these questions, sorting and masking the merged_df.csv on the appropriate columns was done, and the values were interpreted and visualized. The key finding was that there is a weak relationship between the amount of tabacco usage and the decrease in life expectancy in the year 2020. The two variables did not seem to be related as they had a low correlation value of 0.25. 

#### Conclusions and Recommendations

In conclusion, there does not seem to be a correlation between a decrease in life expectancy and tabacco usage in the year 2020. Additionally, the country with the highest tabacco use for 2020 was Myanmar while the country with the lowest life expectancy was Lesotho. However, although there was not a high correlation between the two variables, we know that smoking is very harmful and dangerous and can cause long lasting effects, even if it does not directly lead to death. Smoking should be limited or completely disregarded. For future analysis, the project could be improved upon by adding in another dataset which includes the access to healthcare systems across the world as that plays a huge factor in overall life expectancy. That being said, this data does not take into account how a variety of countries have less access to a good healthcare system. Additionally, the data for tabacco usage in countries only considers adults while there could be a number of underage individuals using the substance, which could also be a further analysis for this project. 
