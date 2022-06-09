# World Weather Analysis

## Overview

The goal of this project was to find a way to provide read-time suggestions for hotels and routes based on preferences in temperature on a vacation.

We started by generating coordinates, then retrieving nearest cities, and then weather descriptions. Then, we had the beta testers use input statements to filter the data for their weather preferences, which was used to identify potential travel destinations and nearby hotels. From the list of potential travel destinations, the beta tester will chose four cities to create a travel itinerary. Finally, using the Google Maps Directions API, we createc a travel route between the four cities as well as a marker layer map.

## Resources
* Python 3.7.13
* VS Code 1.67.2
* Jupyter Notebook

## Results

1. We were able to generage a set of 2000 random latitudes and longitudes, retrieve the nearest city, and perform an API call with the OpenWeatherMap. We used API to retrieve the current weather description for each city. We then created a new DataFrame containing the updated weather data.

2. We created input statements to retrieve customer weather preferences, then used those preferences to identify potential travel destinations and nearby hotels. Then, showed those destinations on a marker layer map with pop-up markers:
![Vacation_Search](https://github.com/bessobrien/World_Weather_Analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

3. We used the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer’s possible travel destinations.
![Route](https://github.com/bessobrien/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

We then created a marker layer map with a pop-up marker for each city on the itinerary:
![Route_with_markers](https://github.com/bessobrien/World_Weather_Analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)

## Summary

We were able to successfully call the API's necessary to provide real-time data based on temperature preferences for a vacation. API's are a useful way to provide data in real time, and by using Python, we can create inputs for those preferences.
