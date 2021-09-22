

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
There were two datasets in this project: one provided by provided by Arvato for this project. 
As part of the terms and conditions of Arvato, the files cannot be shared in this repository. However, they can be described below.

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

- Exploring time-series data

- Use prophet to forecast this time-series as the official doc suggests.

- Extra: showing with data the relation between the animal shelter adoptions and covid mobility restrictions.

## Results
Results here
- Results
- Results
- Results
- Results
- Results
