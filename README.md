# STOR320-Data-Science-Course-Project

This is the final project for STOR 320, Group 1. 

## Introduction
According to the U.S. News’ 10 Most Congested Cities Report, New York City, New York has the fourth highest traffic levels in the United States. The three cities above New York have only slightly more hours that each passenger spends in traffic, while thousands of other United States cities fall substantially below New York’s number. With the clear traffic congestion that exists in New York City, New York, there is a consequential increased risk for traffic accidents.

When contemplating this interest in New York City traffic accidents, we began to wonder how high injury rates are in the area. Furthermore, we began to wonder if traffic could be managed in a way that reduced the possibility of injury or death from an accident. If we could find a pattern among the factors involved in the most deadly accidents, we could understand the most dangerous risk factors for vehicle travel in New York City. This could be further applied to our lives through considering how those factors may be similar in cities closer to us, such as Raleigh, Durham, or Chapel Hill.

## Question
In New York City, will certain vehicle passengers have a higher chance of being killed or injured given the time, location, contributing factors, and vehicle types involved in the traffic accident?

## DataSet: 
The data that is used in this analysis is the NYC Traffic Accidents dataset on Kaggle. The data was collected by the New York City Police Department from January - August of 2020. We use many variables from this data to help with our analysis. The variables we used from this data are: Number of Persons Injured, Number of Persons Killed, Hour, Month, Longitude, Latitude, Contributing Factors 1-5 and Vehicle Type Code 1-5.

## Methods: 
We used a logistic regression model with penalty terms (LASSO and Ridge) to predict whether an accident would have people injured or killed given its location, time, vehicle type involved, and the contributing factors. Moreover, XGBoost are also used to fit the data to see if there is any improvement in accuracy. 

## Results: 
The achieved prediction accuracy is 0.6743 for logistic regression model and 0.7012 for XGBoost model, compared to the No Information Rate 0.5008. The Sensitivity and Specificity is 0.6012 and 0.7471. We also plotted the ROC curve and calculated the AUC score to be 0.7469884, which indicates that our model’s performance is good.

