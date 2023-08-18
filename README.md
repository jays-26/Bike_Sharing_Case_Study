# Bike Sharing Assignment
A bike-sharing system is a service in which bikes are made available for shared use to individuals on a short term basis for a price or free. Many bike share systems allow people to borrow a bike from a "dock" which is usually computer-controlled. The assignment is to understand the factors on which the demand for these shared bikes depends. Specifically, they want to understand the factors affecting the demand for these shared bikes in the American market using Linear Regression.


## Table of Contents
* [General Info](#general-information)
* [Technologies Used](#technologies-used)
* [Conclusions](#conclusions)
* [Acknowledgements](#acknowledgements)

## General Information
# Overview
	* This assignment is a programming assignment wherein we have to build a multiple linear regression model for the prediction of demand for    shared bikes. 
	* BoomBikes is a company who provides system for bike-sharing in which bikes are made available for shared use to individuals on a short term basis for a price or free.
	* The company wants to understand the factors affecting the demand for these shared bikes
	     - Which variables are significant in predicting the demand for shared bikes.
		 - How well those variables describe the bike demands
#background
	A bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue. For that they need to understand the demand for shared bikes among the people, and the factors or variables which affects the demand.
# Business Problem
	You are required to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features, the model will be a good way for management to understand the demand dynamics of a new market. 
# Dataset 
	The dataset given in assignment is day.csv. Where cnt will be used as target variable(where cnt is count of total rental bikes including both casual and registered)
	

## Conclusions
- dataset we have these categorical variables: season ,weathersit, yr, mnth, holiday, weekday, workingday,
  And by seeing the boxplot we can say : 
	1.	Bike demand is high during the fall season and low in spring.
	2.	Bike demand is high if weather is clear or with mist cloudy while it is low when there is light snow or heavy rain.
	3.	In year 2018 the demand was much lower than in 2019.
	4.	Month: The bike demand was lower in the beginning of the year December to March  and on top since June till October, this is also comparable with weathersit.
	5.	Demands are lower on Holidays. 
	6.	Bike Demands found similar during all weekdays and also no significance change based on workingday.
	
- The 3 most important features hum, atemp and mnth , seeing the VIF value and co-efficient. 
- temp and atemp has the highest correlation with the target variable with value .63, and hence dropped temp and kept atemp to build model
- After building model using Linear Regression using RFE we checked the summary and found P values for all the variables is 0 except hum and holiday, which is also very less near to zero.
- The Residual distribution is normal and mean is 0, and scatter plot shows linear relationship between x and y which shows t indicates that the assumptions of a linear regression model are being met.
- R2 score is used to evaluate the performance of a linear regression model, in this case I have calculated the R2 score as .745 ie, 74% accuracy.


## Technologies Used
- Python 3 is used with below libraries:
 pandas numpy pandas numpy matplotlib.pyplot, seaborn, statsmodels,sklearn,and (LinearRegression, r2_score,MinMaxScaler from sklearn)


## Acknowledgements
Give credit here.
- This project was inspired by Upgrad team Module 'Linear Regression'
- References : (https://github.com/ContentUpgrad/Linear-Regression/tree/main/Multiple%20Linear%20Regression%20in%20Python).

## Contact
Created by [@jays-26 - feel free to contact me!
