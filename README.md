# Global Meat Consumption Analysis
## Background
For this analysis, global meat consumption is analyzed.  There has been a growing debate around red meat and its impacts on health.  According to one [study](https://www.sciencedaily.com/releases/2020/02/200203114328.htm) conducted by Northwestern University, higher red meat consumption was linked to higher risks of cardiovascular disease and death.  However, a previous source claimed that red meat does not impact cardiovascular disease risk.  Therefore, for this analysis, we explore global trends to see if countries with higher beef consumption have higher cardiovascular disease death rates.  Furthermore, there recently has been a great deal of interest in the [Mediterranean diet](https://www.mayoclinic.org/healthy-lifestyle/nutrition-and-healthy-eating/in-depth/mediterranean-diet/art-20047801) which is a plant based diet with very little red meat.  This diet is supposed to reduce the risk for cardiovascular disease.  Therefore, we also investigate the trends over time to see if countries are consuming less red meat and becoming more in line with the Mediterranean diet.  

## Business Question
_How has global beef consumption and the cardiovascular death rate changed over time?_

## Data Sources
1. Meat Consumption Worldwide

https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/meat_consumption_worldwide.csv

This data set contains the consumption of beef, poultry, sheep, and pig for many countries from 1990 to 2026 (predicted values).  This data was downloaded from [Kaggle](https://www.kaggle.com/vagifa/meatconsumption).

2. Cardiovascular Disease Death Rates

https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/cardiovascular-disease-death-rates.csv

This data set contains the number of cardiovascular disease deaths per 100,000 people for each country from 1990 to 2017.  This data was downloaded from [Our World in Data](https://ourworldindata.org/grapher/cardiovascular-disease-death-rates). 

3. Meat Consumption in India

https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/Meat_Consumption__India.csv

This data set contains the consumption of beef, poultry, sheep, and pig in India from 1990 to 2026 (predicted values).  This data was downloaded from [Kaggle](https://www.kaggle.com/vagifa/meatconsumption).

4. Meat Consumption in the USA

https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/USA_Meat_Consumption.csv

This data set contains the consumption of beef, poultry, sheep, and pig in the USA from 1990 to 2026 (predicted values).  This data was downloaded from [Kaggle](https://www.kaggle.com/vagifa/meatconsumption).


## Data Analysis

### Beef Consumption Over Time

To answer our question, we first investigate beef consumption from 1991 to 2026 (predicted values)in kilograms per capita.  We focus on six countries for this analysis: three traditionally [high meat consumption countries](https://www.worldatlas.com/articles/top-meat-consuming-countries-in-the-world.html) (Australia, United States, and Israel) and three traditionally [low meat consumption countries](https://www.worldatlas.com/articles/countries-who-consume-the-least-meat.html#:~:text=The%20least%20meat%20consuming%20countries,consuming%20country%20in%20the%20world.) (India, Bangladesh, and Mozambique). 

This graph shows the beef consumption over time for all six countries.  

![alt text](https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/least_and_most_consumption%20(3).png)


In order to get a better idea of the trends, we graph the beef consumption over time for the three high meat consumption countries.  

![alt text](https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/most_consumption%20(3).png)

This graph shows that beef consumption in Israel appears to be on an incline, Australia is on a decline, and the United States appears to be on a very slight decline.  


We also graph the beef consumption over time for the three low meat consumption countries.  

![alt text](https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/least_consumption%20(3).png)

This graph shows that beef consumption in Mozambique is on an incline, Bangladesh is on a slight decline, and India appears to be constant for this year.  

### Cardiovascular Disease Deaths Over Time

We want to explore also explore the cardiovascular disease death.  Therefore, we graph the amount of deaths from cardiovascular disease over time per 100,000 people. We focused on the same six countries for comparison purposes.  

![alt text](https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/heart_death%20(2).png)

Contrary to our expectations, the three low meat consumption countries have higher cardiovascular disease deaths.  


In order to get a better idea of the trends, we graph the cardiovascular disease deaths over time for the three high meat consumption countries.  

![alt text](https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/heart_death_high%20(1).png)

This graph shows that the the cardiovascular disease deaths is decreasing for each of these countries.  This is contradicts the study since Israel has a steep increase in meat consumption but also a steep decrease in cardiovascular deaths.    


We also graph the cardiovascular disease deaths over time for the three low meat consumption countries.  

![alt text](https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/heart_death_low%20(1).png)

This graph shows that the cardiovascular disease deaths is decreasing for Mozambique and Bangladesh and slightly decreasing for India.  This is contrary to the research study since Mozambique has a steep increase in beef consumption but also a steep decrease in cardiovascular disease deaths.  

### Meat Consumption Over Time

Finally, to put the beef consumption trends into context, we graph poultry, sheep, pig, and beef consumption over time for one high meat consumption country (The United States) and one low meat consumption country (India).  

Here is the graph for the poultry, sheep, pig, and beef consumption over time in the United States. 

![alt text](https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/USA_meat_picture.png)

Here is the graph for the poultry, sheep, pig, and beef consumption over time in India. 

![alt text](https://github.com/shannonpowelson/global-meat-consumption-analysis/blob/main/IND_meat_picture.png)

In both of these graphs, poultry consumption is increasing more than the other meats.  

## Summary
Overall, beef consumption over time and cardiovascular disease deaths over time do not appear to have similar trends.  In fact there are trends that contradict the study that claims that higher beef consumption is linked to a higher risk of cardiovascular disease death.  Both Israel and Mozambique contradict this study since they have increasing beef consumption and decreasing cardiovascular disease deaths.  In addition, the three low beef consumption countries have more cardiovascular disease deaths than the three high beef consumption countries.  Therefore, there are likely confounding variables impacting these results.  Also, these graphs alone do not show whether or not countries are adopting a Mediterranean diet (more data on fish and plant consumption is also needed).  Future research on GDP, religion, exercise, and healthcare in these countries over time could provide more insight.  Linear regression should also be used to see if there are any correlations.  This analysis is important for the medical field because it shows that studies on red meat and cardiovascular disease should also take other lifestyle variables into consideration.

## Python Comments
Python was useful in this analysis because we could easily make line graphs showing meat consumption over time.  Also, python allowed for the data set to be isolated based on meat or country which was also useful for these visualizations.  However, vlookup from excel could have added to this analysis since then the cardiovascular disease death rates and the meat consumption could be plotted on the same chart even though they were originally from different excel spreadsheets.  
