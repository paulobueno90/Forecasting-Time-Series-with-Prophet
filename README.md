

<p align="center">
    <img src="image.jpg" alt>
</p>

# Forecasting Using Prophet

---

The following project has been created as part of my learning path, seeking to understand one of the well known framework for time-series forecasting.

**Prophet** is a forecasting framework for time series, made available as an open source project by Facebook. Implemented in Python and R, it is capable of performing automated and fast forecasts.

To access the project's official documentation: [Prophet Official Doc Page.](https://facebook.github.io/prophet/)

---

## Libraries Used

Python Version: 3.7.12 

- Pandas
- Matplotlib
- Scikit-Learn
- statsmodels
- sodapy [API for Austin Texas Gov Data](https://dev.socrata.com/foundry/data.austintexas.gov/9t4d-g238)
- fbprophet

## File Descriptions
There were four data files provided by Arvato for this project. 
As part of the terms and conditions of Arvato, the files cannot be shared in this repository. However, they can be described below.

#### Demographics data

##### austin.xlsx -  MEI data
- 891,211 rows
- 366 features

##### customers.csv - customers of a mail-order company 
- 191,652 rows
- 369 features

##### mailout_train.csv - target individuals of a marketing campaign (train) 
- 42,982 rows
- 367 features

##### mailout_test.csv - target individuals of a marketing campaign (test) 
- 42,833 rows
- 366 features

## Notebooks Description
These are public notebooks and can be used.
- 1-DataExploration_and_Cleaning.ipynb: Notebook data preparations such as cleaning, feature engeneering and handling NaNs
- 2-Customer Segmentation.ipynb: Notebook initiates with clean data and go to steps of dimensionality reduction and clustering
- 3-Supervised Model.ipynb: Test models, fit and submission.
## Python Functions
- functions.py - File with some functions used in the notebooks.

## Summary
This challenge was provided by Arvato Financial Solutions for the Udacity Data Science Nanodegree Program.
There were two major steps in the project and the submission

#### Customer Segmentation Report 
With data of customers of a mail-order sales company in Germany and comparing it with demographics information for the general population. In this part it is used unsupervised learning techniques to perform customer segmentation, identifying through clusters the parts of the population that best describe the customer of the company.

#### Supervised Learning Model
This part it is used the knowledge from the previous analysis and a machine learning model is build to predict whether or not a person will become a customer.

#### Kaggle Competition 
With the model created, it is time to submit the predictions of the test data to this [Kaggle Competition](https://www.kaggle.com/c/udacity-arvato-identify-customers)

## Results
There are a lot of features missing description which was needed further investigation but i didn't have the time to adress. Therefore in summary, looking into data it can be said that the group of potencial customers are likely to have these characteristics:
- Individuals with Higher income and wealth.
- Individuals which is more avantgard than mainstream and more likely to be green avantgarde ( sustainability)
- Live in areas with lower density of inhabitants and lower unemployement.
- Has higher mobility
- Mid-ager with family individuals

If the company were willing to launch a marketing campaign, it would be more efficient to target these clusters of characteristics.

## Acknowledgements

Udacity - For giving me the opportunity to learn and develop with real projects

Arvato - For the oppotunity to work on their data with a real life project experience


