# Regression-Bike-Sharing-Demand-Prediction

Table of Content

Introduction

Problem Statement 

Dataset Information
Tools and Technologies used

Steps involved

Algorithms used

Conclusion

**Introduction**

Bike sharing system is an innovative transportation strategy that provides individuals with bikes for their common use on a short-term basis for a price or for free. Over the last few decades, there has been a significant increase in the popularity of bike-sharing systems all over the world. This is because it is an environmentally sustainable, convenient and economical way of improving urban mobility. In addition to this, this system also helps to promote healthier habits among its users and reduce fuel consumption.


🎯 **The goals of this project are:**

Understand the trends in the data and identify key factors affecting the hourly demand for rental bikes.

Build an appropriate regression model to forecast the number of rental bikes required per hour.


**Problem Statement**

Currently Rental bikes are introduced in many urban cities for the enhancement of mobility comfort. It is important to make the rental bike available and accessible to the public at the right time as it lessens the waiting time. Eventually, providing the city with a stable supply of rental bikes becomes a major concern. The crucial part is the prediction of bike count required at each hour for the stable supply of rental bikes.

-----------------------------------------------------

📖 **Dataset information**

Dataset used in this project is the Seoul Bike Share program data.This dataset contains information about 
the total count of rented bikes at each hour, 

as well as the date of observation and meteorological information (Humidity, Snowfall, Rainfall, Temperature Season, and so on) for that hour.

The observations in the dataset were recorded during a span of 365 days, from December 2017 to November 2018.


The Seoul Bike Dataset contains the following information:


Date - The date of each observation in the format 'year-month-day'

Hour - Hour of the day

Temperature - Temperature recorded in the city in Celsius (°C).

Humidity - Relative humidity in %

Wind speed - Speed of the wind in m/s

Visibility - measure of distance at which object or light can be clearly discerned in units of 10m

Dew point temperature - Temperature recorded in the beginning of the day in Celsius(°C).

Solar radiation - Intensity of sunlight in MJ/m^2

Rainfall - Amount of rainfall received in mm

Snowfall - Amount of snowfall received in cm

Seasons - Season of the year (Winter, Spring, Summer, Autumn)

Holiday - Whether the day is a Holiday or not (Holiday/No holiday)

Functional Day -Whether the rental service is available (Yes-Functional hours) or not (No-Non functional hours)

Rented Bike count - Count of bikes rented at each hour (target variable)
-----------------------------------------------------

🛠️ **Tools and Technologies used**

The programming language used in this project is Python . The following libraries were used for data analysis and data visualization and to build a classifier to predict the price range of mobile phones.

Pandas : For loading the dataset and performing data wrangling

Matplotlib: For data visualization.

Seaborn: For data visualization.

NumPy: For some math operations in predictions.

Statsmodels: For statistical computations

Sklearn: For the purpose of analysis,prediction and evaluation.
-----------------------------------------------------

📑 **Steps involved**

Data Preprocessing : Checked for outliers, incorrect values, missing values, duplicates and performed data type correction.

Feature Extraction : Created new columns such as Day, Month, Year, Days_of_week and Weekend from Date column .

Exploratory Data Analysis : Performed Univariate, Bivariate, and Multivariate analysis with various graphs and plots to better understand the distribution of features and their relationships.

Feature encoding : The categorical features present in the dataset Seasons, Holiday, Weekend, Functioning Day were dummified.

Feature Scaling : Brought features to a similar range using MinmaxScaler.

Implementation of Regression models

Comparison of models
-----------------------------------------------------

💻 **Algorithms used**

Linear Regression

Lasso Regression

Ridge Regression

Decision Tree

**Conclusion**

**Findings from EDA:**

Temperature and Hour have a strong correlation with the count of rented bikes.

Dew point temperature is highly positively correlated to the Temperature.

Over the weekend and during holidays, rental bike demand decreases.

There is a significant drop in the number of rented bikes during Winters(Dec-Feb) because it's freezing cold!

The demand for bikes increases during warmer temperatures,which is why there's maximum count of rented bikes during the Summer season.

In all seasons,the peak demands for rental bikes occur on the opening (8-9 AM) and closing times (6-7pm) of offices and institutions.

**Conclusion Based on Model Evaluation:**

Stacking was found to be most suitable for making predictions of hourly demand for rental bikes.

Temperature and Hour were found to be most influential variables in predicting the hourly demand for rental bikes.

When compared to other models used, decision tree-based models have performed well.

















