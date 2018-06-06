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
- Quality of Life (‘Drugs’, ‘Liquor’,'Other','Traffic','Disorder','Quality of Life','Fire') 
- Property ('Property Crime','Theft', 'Theft of Vehicle', 'Theft from Vehicle') 
- Violent ('Assault’,'Assault with Deadly Weapon','Homicide','Kidnapping','Other Sexual Offense','Sexual Assault','Sexual Offense')

Forecasted crime rates in all 3 categories for a strabucks store in seattle.

Following are the forecasted crime rate trends (monthly,yearly,weekly and daily trends) for that store:

1. Quality of Life Crimes (‘Drugs’, ‘Liquor’,'Other','Traffic','Disorder','Quality of Life','Fire')

![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/QualityOne.PNG)
![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/QualityTwo.PNG)<br/>

Interesting Observations:
- daily plot shows that Quality of Life crimes for this store happen mostly around early morning 4 and  at evening 8pm
- weekly plot shows that these crimes around this store happen mostly on Fridays<br/>

Forecasted values: <br/>
![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/Tier1_Forecasted_Values.PNG)

2.Property Crimes ('Property Crime','Theft', 'Theft of Vehicle', 'Theft from Vehicle') 

![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/PropertyOne.PNG)
![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/PropertyTwo.PNG)<br/>

Interesting Observations:
- daily plot shows that Property Crimes for this store happen mostly around 12am 
- weekly plot shows that Property Crimes for this store happen mostly on Thursdays<br/>

Forecasted values: <br/>
![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/Tier2_Forecasted_Values.PNG)

Note : yhat is the predicted value , yhat_lower is the lower range , yhat_upper is the upper range<br/>

For example "2018-11-30" has 12 predicted crime values and it lies between 4 and 40. where 12 is yhat value and 4 is yhat_lower value and 40 is yhat_upper value 

3.Violent Crimes ('Assault’,'Assault with Deadly Weapon','Homicide','Kidnapping','Other Sexual Offense','Sexual Assault','Sexual Offense')

![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/ViolentOne.PNG)
![alt text](https://github.com/LalithaPalleti/Starbucks-Security-Analysis-and-Forecasting/blob/master/ViolentTwo.PNG)<br/>

Interesting Observations:
- All the plots are staright lines because there is no crime data for Violent Crimes. I went to the datasource and checked that there are only three tier3 Incidents in the whole seattle area<br/>

Forecasted values: <br/>
Zero<br/>

This may be due to lack of violent crimes data in the crimereports.com .If extracted from a different data source might bring more values 

