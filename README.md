# Project Name
Bike Sharing Linear Regression Assignment
> Requirement to model the demand for shared bikes with the available independent variables. It will be used by the management to understand how exactly the demands vary with different features. They can accordingly manipulate the business strategy to meet the demand levels and meet the customer's expectations. Further, the model will be a good way for management to understand the demand dynamics of a new market.


## General Information
- Provide general information about your project here. - Need to identify the demand for a bike sharing platform based on multiple categprical nd some continuous variables
- What is the background of your project? - A US bike-sharing provider BoomBikes has recently suffered considerable dips in their revenues due to the ongoing Corona pandemic. The company is finding it very difficult to sustain in the current market scenario. So, it has decided to come up with a mindful business plan to be able to accelerate its revenue as soon as the ongoing lockdown comes to an end, and the economy restores to a healthy state. 
In such an attempt, BoomBikes aspires to understand the demand for shared bikes among the people after this ongoing quarantine situation ends across the nation due to Covid-19. They have planned this to prepare themselves to cater to the people's needs once the situation gets better all around and stand out from other service providers and make huge profits.
- What is the business probem that your project is trying to solve?
- What is the dataset that is being used?
  day.csv have the following fields:
	
	- instant: record index
	- dteday : date
	- season : season (1:spring, 2:summer, 3:fall, 4:winter)
	- yr : year (0: 2018, 1:2019)
	- mnth : month ( 1 to 12)
	- holiday : weather day is a holiday or not (extracted from http://dchr.dc.gov/page/holiday-schedule)
	- weekday : day of the week
	- workingday : if day is neither weekend nor holiday is 1, otherwise is 0.
	+ weathersit : 
		- 1: Clear, Few clouds, Partly cloudy, Partly cloudy
		- 2: Mist + Cloudy, Mist + Broken clouds, Mist + Few clouds, Mist
		- 3: Light Snow, Light Rain + Thunderstorm + Scattered clouds, Light Rain + Scattered clouds
		- 4: Heavy Rain + Ice Pallets + Thunderstorm + Mist, Snow + Fog
	- temp : temperature in Celsius
	- atemp: feeling temperature in Celsius
	- hum: humidity
	- windspeed: wind speed
	- casual: count of casual users
	- registered: count of registered users
	- cnt: count of total rental bikes including both casual and registered

## Steps to be followed
1. Understanding the data
2. Preparation - Test-Train, Scaling
3. Training Dataset
4. Residual Analysis
5. Prediction and model evaluation

## Conclusions
- The equation of the best fitted line is:
cnt = 0.075 + 0.233*yr + 0.0561*workingday + 0.55*temp - 0.15*windspeed + 0.08*season_2 + 0.13*season_4 + 0.97*weekday_6 - 0.08*weathersit_2 - 0.287*weathersit_3


## Technologies Used
- packages used: sklearn, matplotlib, seaborn, statsmodels, pandas, numpy
