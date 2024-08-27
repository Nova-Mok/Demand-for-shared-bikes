# Bike Demand Prediction

A Jupyter Notebook for predicting the demand for shared bikes using multiple linear regression. This project is designed to help understand the factors that influence bike-sharing demand based on historical data.

## Table of Contents
- [General Information](#general-information)
- [Dataset](#dataset)
- [Installation](#installation)
- [Usage](#usage)
- [Model Building](#model-building)
- [Results](#results)

## General Information

Bike-sharing systems are a popular mode of transportation in urban areas, providing a flexible and eco-friendly way to commute. This project aims to build a predictive model to estimate bike demand based on various factors such as weather, season, and time of year.

Understanding bike demand helps operators manage resources efficiently, optimize bike distribution, and enhance user experience.

## Dataset

The dataset used for this project contains daily bike rental counts and various attributes that might affect bike usage. The dataset includes the following fields:
- **instant**: Record index
- **dteday**: Date
- **season**: Season (1: spring, 2: summer, 3: fall, 4: winter)
- **yr**: Year (0: 2018, 1: 2019)
- **mnth**: Month (1 to 12)
- **holiday**: Whether the day is a holiday or not
- **weekday**: Day of the week
- **workingday**: Whether the day is neither weekend nor holiday
- **weathersit**: Weather situation (1: Clear, 2: Mist, 3: Light Snow/Rain, 4: Heavy Rain)
- **temp**: Normalized temperature in Celsius
- **atemp**: Normalized feeling temperature in Celsius
- **hum**: Normalized humidity
- **windspeed**: Normalized wind speed
- **casual**: Count of casual users
- **registered**: Count of registered users
- **cnt**: Count of total rental bikes including both casual and registered users

## Installation

To run this project, you will need to install the following dependencies:

- Python 3.x
- pandas
- numpy
- matplotlib
- seaborn
- scikit-learn
- statsmodels
- scipy

## Model Building

The project involves the following steps:

Data Loading: Load the dataset and perform initial data exploration.
Data Preprocessing: Convert categorical variables, handle missing values, and create dummy variables.
Feature Selection: Drop irrelevant features and handle multicollinearity using Variance Inflation Factor (VIF).
Model Training: Train a multiple linear regression model using the processed dataset.
Model Evaluation: Evaluate the model using metrics like R-squared and perform residual analysis to validate the model assumptions.


## Results

The model's R-squared score on the test data is 0.83, 
indicating that the model explains about 83% of the variability in bike demand based on the provided features. 
Key factors influencing bike demand include temperature, season, and working day.
