# Module6Challenge
## Overview of Project
Mytrip is a top travel technology company that specializes in internet related services in the hotel and lodging industry. Jack, head of analysis of the user interface team, has requested help with collecting and presenting data for customers via the search page. The goal is to collect and analyze weather data across cities worldwide so that Mytrip can launch the app PlanMyTrip. PlanMyTrip will be used to recommend ideal hotels based on clients' weather preferences and create a travel itinerary between four cities of choice. 

## Objectives
* Use the NumPy module to generate more than 2,00 random latitudes and longitudes.
* Use the citipy module to list the nearest city to the latitudes and longitudes.
* Use the OpenWeatherMap API to request the current weather data from each unique city in your list.
* Parse the JSON data from the API request.
* Collect the following data from the JSON file and add it to a DataFrame:
    * City, country, and date
    * Latitude and longitude
    * Maximum temperature
    * Humidity
    * Cloudiness
    * Wind speed
    * Current weather description
* Create visuals with travel data via a heatmap with pop-up markers that can display information on specific cities based on a customer's travel preferences. 
    * Filter the Pandas DataFrame based on user inputs for a minimum and maximum temperature.
    * Create a heatmap for the new DataFrame.
    * Find a hotel from the cities' coordinates using Google's Maps and Places API, and Search Nearby feature.
    * Store the name of the first hotel in the DataFrame.
    * Add pop-up markers to the heatmap that display information about the city, current weather conditions, and a hotel in the city.
* Use the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer's possible travel destinations. Then create a marker layer map with a pop-up marker for each city on the itinerary.


# Development Environment 
* Jupyter Notebook
* Python v3.10.4 Dependencies:
  * Python Pandas library
  * Python Numpy library
  * Python Matplotlib.pyplot library 
  * Scipy.stats module
  * Citipy library
  * Time library
  * Requests library
  * gmaps

# Data Sources
* [citypy](https://github.com/wingchen/citipy)
* [jupyter - gmaps](https://jupyter-gmaps.readthedocs.io/en/latest/)
* [OpenWeatherMap API - Current Weather](https://openweathermap.org/current)
* [Google API - Place Search](https://developers.google.com/maps/documentation/places/web-service/search)
* [Google API - Directions API](https://developers.google.com/maps/documentation/directions/overview)

## Results

# Retrieve Weather Data
Generated a set 2,000 random latitudes and longitudes, retrieved the nearest city, and performed an API call with the OpenWeatherMap. Used the API to retrieve the current weather description for each city and created a new DataFrame containing the updated weather data.

![Screenshot 2022-04-17 010757](https://user-images.githubusercontent.com/57520471/163701373-41b67d27-7160-497d-8b3a-21453124b9c0.png)

# Customer Travel Destinations Map
Used input statements to retrieve customer weather preferences and used those preferences to identify potential travel destinations and nearby hotels. Visualized the potential travel destinations on a marker map with pop-markers.

![WeatherPy_vacation_map](https://user-images.githubusercontent.com/57520471/163701418-f8ec05e2-0e59-43ab-9744-dcae76af76d3.png)

## Travel Itinerary Map
Used the Google Directions API to create a travel itinerary that shows the route between four cities chosen from the customer's potential travel destinations. Then created a marker layer map with a pop-up marker for each city on the itinerary.

![WeatherPy_travel_map](https://user-images.githubusercontent.com/57520471/163701455-94606c69-c5a5-478e-bd9b-edd5deb0c5fe.png)

![WeatherPy_travel_map_markers](https://user-images.githubusercontent.com/57520471/163701456-9a12b0fc-8764-437f-8784-70c7aad58dea.png)
