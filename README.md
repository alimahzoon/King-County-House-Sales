# Module 2 Final Project: Predicting homes in kings county

## Introduction

Student name: Joey Husney
Student pace: full time
Scheduled project review date/time: N/A
Instructor name: Yish Lim


As a real estate agency, our goal is to give recommendations to customers on how to increase the value of their home. This will be done through analyzing the data in the "King County House Sales" dataset and investigating which features are correlated with higher sales prices. Using the OSEMN process, we hope to give suggestions that are meaningful and reliable. The OSEMN framework consists of an iterative process of Obtaining the data, Scrubbing it, Exploring, Modeling, and iNterpreting the data into meaningful suggestions for the client.


## The Data
The king county house sales dataset contains data from houses in the Seattle Washington area sold between the time period May 2014 - May 2015. The following features are contained in this dataset:
* **id** - unique identified for a house
* **dateDate** - house was sold
* **pricePrice** -  is prediction target
* **bedroomsNumber** -  of Bedrooms/House
* **bathroomsNumber** -  of bathrooms/bedrooms
* **sqft_livingsquare** -  footage of the home
* **sqft_lotsquare** -  footage of the lot
* **floorsTotal** -  floors (levels) in house
* **waterfront** - House which has a view to a waterfront
* **view** - Has been viewed
* **condition** - How good the condition is ( Overall )
* **grade** - overall grade given to the housing unit, based on King County grading system
* **sqft_above** - square footage of house apart from basement
* **sqft_basement** - square footage of the basement
* **yr_built** - Built Year
* **yr_renovated** - Year when house was renovated
* **zipcode** - zip
* **lat** - Latitude coordinate
* **long** - Longitude coordinate
* **sqft_living15** - The square footage of interior housing living space for the nearest 15 neighbors
* **sqft_lot15** - The square footage of the land lots of the nearest 15 neighbors

## OSEMN Process
- Obtain
- Scrub
- Explore
- Model
- Interpret

## Purpose / Goal
The goal of this project is give meaningful suggestions to our clients on how to increase the value of their home

## Final Modeling
![alt text](https://github.com/alimahazoon/King-County-House-Sales/blob/joey/model.png?raw=true)
![alt text](https://github.com/alimahazoon/King-County-House-Sales/blob/joey/coefs.png?raw=true)
![alt text](https://github.com/alimahazoon/King-County-House-Sales/blob/joey/plots.png?raw=true)
### Recommendations 
- We have found that square footage is key in raising market selling price, therefore people should try to maximize the square footage of their home to increase their value
- We recommend that all of our customers increase the condition of their home. Each point increase in condition increases the value of the home on average by $25,200
- Putting a good number of bathrooms is proven to be a good way of increasing home value
