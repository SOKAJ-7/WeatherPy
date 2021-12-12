# WeatherPy and Google Maps

## Project Overview
The purpose of this project was to use python and application programming interfaces (API) to allow the design of a roadtrip to suit the climate preferences of potential customers. Firstly, numpy and citypy modules were used to randomnly generate a set of 2000 random coordinates and then associate those coordinates with their respective cities. Then, OpenWeatherMaps API was used to create a dataframe (city_data_df) containing the weather data of each of the cities which were generated at random. 

Next, we used the city_data dataframe to filter cities based on minimum and maximum temperatures to narrow the list of potential cities to include in the ideal roadtrip for a prospective client. In this project, the range of 70-90 F was used. This was save as a new dataframe (preferred_cities_df) and used with the Google maps API to associate a hotel within 5000 metres of each city in the new dataframe. A map was then created with markers on each city in the dataframe including each cities' name, country, current weather, and maximum temperature.

The last part of this project was to identify four cities within a driveable distance of each other to create a roadtrip itinerary. Based on our criteria, the Brazilian cities of Palmas, Raposa, Canarana, and Vila Velha were selected. The coordinates of each of these cities were extracted from the preferred cities dataframe as tuples and were used with the google maps directions API to create a map showing the fastest driving route to stop in each city, starting in Palmas and ending in the same location.

This program now can be used for customers to design their own roadtrip based on their climate preferences, how exciting!
