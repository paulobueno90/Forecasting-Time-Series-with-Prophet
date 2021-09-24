

<p align="center">
    <img src="image.jpg" alt>
</p>

# Forecasting Using Prophet


The following project has been created as part of my learning path, seeking to understand one of the well known framework for time-series forecasting.

**Prophet** is a forecasting framework for time series, made available as an open source project by Facebook. Implemented in Python and R, it is capable of performing automated and fast forecasts.

To access the project's official documentation: [Prophet Official Doc Page.](https://facebook.github.io/prophet/)

Data used on this project was made available by the [Austin Animal Center](http://www.austintexas.gov/content/austin-animal-center)and can be downloaded: 
- Directly from the [City of Austin Open Data Portal](https://data.austintexas.gov/Health-and-Community-Services/Austin-Animal-Center-Outcomes/9t4d-g238)
- Using [Austin API](https://dev.socrata.com/foundry/data.austintexas.gov/9t4d-g238)


## Libraries Used

Python Version: 3.7.12 

- Pandas
- Matplotlib
- Scikit-Learn
- statsmodels
- sodapy [API for Austin Texas Gov Data](https://dev.socrata.com/foundry/data.austintexas.gov/9t4d-g238)
- fbprophet

## File Descriptions
There were two datasets used in this project: 

##### austin.xlsx -  MEI data ( weekly data) - ['Mobility and Engagement Index'](https://www.dallasfed.org/research/mei)
- 65 rows
- 7 features
- Feature used: 'Austin-Round Rock-Georgetown, TX'

##### Data from "data.austintexas.gov" API - [Austin Animal Center](http://www.austintexas.gov/content/austin-animal-center)
- 131,000 rows
- 12 features


## Notebooks Description
This is public notebook and can be used.
- Animal_Shelter.ipynb: Notebook with basic time-series exploration, forecasting with prophet and quick correlation between covid restrictions and adoptions 


## Summary
This project was made thinking on learning how to use prophet for time-series tasks, although it couldn't achieve an excellent performance, it was worthy the exercise and visualization. There were 3 steps in this project.

- Explore and identify patterns during the time-series analysis.

- Implement Prophet(following official doc suggestion) to forecast the outcomes of this time-series.

- Extra: showing with data the relation between the animal shelter adoptions and covid mobility restrictions.

## Results
Prophet is very easy and simple to use, and can be used to check time series data, which can get rich insights and hints based on variation of values by day of the week and also possible to clearly identify the seasonality of the months in a faster way.

It is necessary to adress some points:

- larger temporal windows, for example the test with weekly frequency performed considerably better than using the daily frequency. This can be explained by a higher amount of noise contained in series with higher frequency.

- Prophet needs seasonality and trend, meaning that external/unexpected events will make Prophet predictions fail as autocorrelation changes in the short term. If a model needs to capture external events, models created by Prophet is not a good choice.

- [Mobility and Engagement Index](https://www.dallasfed.org/research/mei): Although it was developed as a way to measure activity but with economic purposes, this index has a high correlation with adoption numbers. This index was discontinued on March 31, 2021 which is a shame because I can imagine many other uses and analyzes using it.
