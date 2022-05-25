# World Weather Analysis

## Overview
To use APIs to find weather and maps for cities based on randomly generated geographical coordinates for the purpose of allowing travelers to input their ideal temperature range and select a destination that fits the criteria.
## Process
- Randomly generated geographic coordinates using numPy random.uniform() function
- Used citiPy to find if there were cities near the geographic coordinates
- Used OpeneWEatherMap API to find weather conditions for each of the cities
- Plotted latitude vs max temperatures, humidity, wind speeds and cloudiness and used linear regression to determine if any correlations
- Used google maps API to find a hotel in each city and to create heatmaps
- Requested input from users on idea temperature range and used that to tailor the cities that would appear on the map
- Created a travel itinerary around Brazil
## Resources
- Software: Jupyter Notebooks, conda 4.12.0, Python 3.7.2
- APIs - OpenWeathermap (https://openweathermap.org/api) and Google Cloud Places and Directions 
## Results
The clearest correlation between lattitude and a weather feature was with temperature. As expected, temperatures nearer the equator (0 degrees) were the warmest and temperatures cooled as the reached the poles. There was some observations that cloudiness seemed heavier over the poles, but without looking at a longer time period it would be difficult to determine if this was a strong correlation.
![Fig1](https://user-images.githubusercontent.com/101822948/170334683-c3115628-24cc-4cae-8e37-e9bd30a88a88.png)
![Cloudiness_lat](https://user-images.githubusercontent.com/101822948/170334803-4998990f-34b2-4451-abd3-9d13a2e97205.png)

In regards to trip planning, we were able to narrow cities down by user input into their ideal temperature range and create a map with pop up markers displaying the city, hotels, and weather conditions.

![WeatheryPy_vacation_map](https://user-images.githubusercontent.com/101822948/170335141-8640a435-aa02-4bd2-805a-39fc3a15c579.png)
