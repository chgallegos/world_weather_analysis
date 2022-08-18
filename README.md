# WORLD WEATHER ANALYSIS
----
## Overview

The purpose of this exercise is to engage with the use of APIs by the creation of a database based on 2,000 random latitudes and longitudes. This database was subsequently used in the development of two tools, a hotel search tool based on temperature preferences and an itinerary based on directions.


----
## Results
### PART 1 "Weather Database"
The analizis began by creating a database using random combinations of latitudes and longitudes.
![Screenshot](https://github.com/chgallegos/world_weather_analysis/blob/main/resources/lats_lngs_random.png)

The next step was an API call requesting city and weather data for all of those combinations
![Screenshot](https://github.com/chgallegos/world_weather_analysis/blob/main/resources/combinations_API_calls.png)

the final part of this process was to create a DataFrame with the requested information and save into a .csv file to be used in the next tool.

### PART 2 "Vacation Search"

The purpose of this tool is to allow the customer input temperature preferences in order to provide locations and hotels. In this case, another API call was used in Google Places "nearby search". This API provides the customer with hotel locations based on the latitudes and longitudes provided by their temperature preferences. It also stores the narrowed search in a new dataframe.
![Screenshot](https://github.com/chgallegos/world_weather_analysis/blob/main/resources/nearby_search_API_calls.png)

For the user experience end of things, the tool provides a map with markers for the recommended hotels as well as a box with relevant information.
![screenshot](https://github.com/chgallegos/world_weather_analysis/blob/main/Vacation_Search/WeatherPy_vacation_map.png)

### PART 3 "Vacation Itinerary"

From the dataframe created in Part 2, a selection of 4 cities is made in order to provide a route itinerary with the use of the Gmaps directions layer.
![screenshot](https://github.com/chgallegos/world_weather_analysis/blob/main/resources/driving_directions.png)

User interface provides the product for the customer:
![screenshot](https://github.com/chgallegos/world_weather_analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map.png)

Finally, a map with information boxes for all of the locations is generated. This information is relevant to the customer's search.

![screenshot](https://github.com/chgallegos/world_weather_analysis/blob/main/Vacation_Itinerary/WeatherPy_travel_map_markers.png)
----
## Summary 

This exercise showed the fundamental importance of managing APIs and how they have the ability to provide a significant value to customers. It also allowed for the exploration of API documentation, this is also a fundamental ability to develop since APIs have the ability to provide an enormous amount of information that, if used wisely, can provide a stellar customer experience.