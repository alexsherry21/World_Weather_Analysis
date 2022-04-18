# World_Weather_Analysis
Python/API work for module 6

## Overview
In Module 6 we help create an app for PlanMyTrip.  We use Python with Pandas, NumPy, and API calls in order to assist customers in finding destinations that meet their desires.

### Results
Our goal was to help customers find where they might best like to vacation.  We decided to take customer input on a range for desired maximum temperature which was used to filter our set of cities and hotels that we acquired through the OpenWeatherMap and Google Maps and Places APIs.  For example, here is a marker map of cities with a maximum temperature today between seventy-five and ninety degrees Fahrenheit.

![WeatherPy_vacation_map](https://user-images.githubusercontent.com/100380226/163750359-b2246ad6-a6bd-47d5-a616-25b2252a3991.png)

We additionally used the Google Directions API to put together a sample trip for a customer interested in vacationing in Brazil.

![WeatherPy_travel_map](https://user-images.githubusercontent.com/100380226/163750481-a38d53cf-2b23-49c8-b2db-2ba647ecdab0.png)

We are able to select any four cities in our DataFrame and output a route that loops back to the starting point.  Additionally, we put together many scatter plots from our data as a side project for local students to use in their climate analysis.

![Fig1](https://user-images.githubusercontent.com/100380226/163750605-5d283cd4-b227-4ddb-bded-70f667ee930e.png)

### Summary
PlanMyTrip now has a basis on which to build an app to help customers find their perfect vacations.  One thing that stood out to me was that we took latitudes and longitudes entirely at random.  Because most of the surface of the Earth is water, we expect that roughly seventy percent of the coordinates we pull to be over bodies of water.  This leads to an oversampling of coastal cities.  While many people prefer to vacation on the coast,  PlanMyTrip should also want to capitalize on demand for trips to ski resorts, national parks and monuments, major sporting events and concerts, and other major sources of travel that are not necessarily located near the coasts.  If Google's APIs can detect whether a point is over land or water, we could restrict coordinates to obtain a more even sampling.
