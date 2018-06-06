# Starbucks-Security-Analysis-and-Forecasting
## Introduction
Crime investigation around Starbucks Stores in Seattle

This project's goal is to collect crime history data around certain starbucks stores in seattle area and categorize the level of crimes by their crime type and forecast the future crime rates and category in which each store falls and therfore take security measures at each store accordingly 

## Model
Crime data in seattle area is extracted from   https://www.crimereports.com/

Used Facebook's Prophet model to forecast crime rates around starbucks stores in seattle area

First I have trained the Prophet model using the crime data in the seattle area.
Then I forecasted for future 6 months of data using prophet's predict method.

## Results
Crime severity is divided into 3 categories: 
- Quality of Life (‘Drugs’, ‘Liquor’,'Other','Traffic','Disorder','Quality of Life','Fire'), 
- Property ('Property Crime','Theft', 'Theft of Vehicle', 'Theft from Vehicle'), 
- Violent ('Assault’,'Assault with Deadly Weapon','Homicide','Kidnapping','Other Sexual Offense','Sexual Assault','Sexual Offense')

Forecasted crime rates in all 3 categories for a strabucks store in seattle.

Following are the forecasted crime rate trends (monthly,yearly,weekly and daily trends) for that store:

1. Quality of Life Crimes

![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/QualityOne.PNG)
![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/QualityTwo.PNG)
![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/Tier1_Forecasted_Values.PNG)

2.Property Crimes

![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/PropertyOne.PNG)
![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/PropertyTwo.PNG)
![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/Tier2_Forecasted_Values.PNG)


3.Violent Crimes

![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/ViolentOne.PNG)
![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/ViolentTwo.PNG)
![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/Tier3_Forecasted_Values.PNG)

