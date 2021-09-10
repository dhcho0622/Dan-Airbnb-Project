# Airbnb Pricing Linear Regression Model

Airbnb Project:
By: **Daniel Cho**

## Introduction

Airbnb has been one of the fastest growing startups of this century. Creating an entirely new way of traveling, Airbnb has built its company by offering their customers a home away from home. One of the biggest areas of opportunity is that Airbnb listings are largely managed by non-professionals. This causes huge price variances as most hosts are not knowledgable on how to correctly price each night of their listing. The purpose of this project is to create a model to better predict what pricing should be on a given listing in NYC.

I pulled my data from two sources:
 1. Kaggle Open Source Airbnb Data that contained over 40000+ listings in NYC on Airbnb
 2. Crime Data from data.cityofnewyork.us in NYC for all of 2019 (200000+ recorded arrests information)

From here I posed 4 questions I wanted to focus my analysis:
 1. What data features best impact my modeling and what they show?
 2. What statistical testing explains about different hypothesis of my data?
 3. How data visualizations portray certain trends within my model?
 4. Which model best fits for future testing?
    - How would I price my own apartment?
 
## Files in this Repository
 * Final Cleaning & Modeling.ipynb.ipynb:
    - Data Cleaning of Airbnb Data & API of NYC crime statistics
    - Multi Regression
    - Statistical Testing (2 sample T Test, One Way ANOVA, Chi Squared)
    - Modeling & Feature Engineering (Dummy Variables, Polynomials, F-Test, Recursive)
 * Test Results from Model.ipynb:
    - Pickled(saved) my best fit model to help predict how to price my own apartment in Long Island City
 * PNG Visuals - Folder contained png files of all data visualizations
 * CSV files containing the data sets, merged, and cleaned

## Built with Libraries
**Data Collection**
 * Pandas
 * NumPy
 * Requests
 * Json
 * Scipy
 * Matplotlib
 * Seaborn
 * Statsmodels
 * Sklean
 
## Limitations and Further Exploration
**Limitations**

The biggest limitation for this model is the pricing data scraped from Airbnb
* Pricing from data set can be representative of entirely different days. (Airbnb shows the 1st available price therefore we are not able to factor in day of week or seasonality price)
* Because of this, my model is predicitng the baseline value for a nightly rate not a dynamic rate based on demand
* Airbnb rentals have so many unique and extreme outliers compared to traditional hotels
* There were very few strong indicators of correlation on the features further illustrating the complexities of predicting daily pricing

**Further Exploration**

* Airbnb lacks reliable square footage data which could be a useful feature
* Pulling pricing data from professional Airbnb rental companies such as Sonder or Domio to provide a better baseline
* Utilize more location based features such as distance from landmarks, subways, attractions
* Focus more on just Manhattan and Brooklyn as over 90% of listings are from just those two boroughs
* Submit Project to Airbnb for potential review and introdution
## Presentation 

https://docs.google.com/presentation/d/1JBytZzNBUcXgbpcD_PzXNnfx5TFPMUTslyT4zGMAOpY/edit#slide=id.p
