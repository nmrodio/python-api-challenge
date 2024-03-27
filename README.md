# **python-api-challenge** #
--------

## **Project Goal** ##
This project explores the intersection of geospatial data analysis and hospitality information retrieval using public Application Programming Interfaces (APIs) and demonstrates the power of APIs in combining geospatial data with hospitality information to create a user-centric recommendation system.

**Data Acquisition:**

 * **Geolocation Data:** The project utilizes the Geoapify API (https://www.geoapify.com/) to retrieve latitude coordinates for various randomly selected cities.
* **Weather Data:** OpenWeatherMap's API (https://openweathermap.org/api) provides weather metrics including maximum temperature, humidity, cloudiness, and wind speed for these cities. Both sets of data are retrieved in JSON format.

**Analysis:**

The project investigates potential linear relationships between a city's latitude and the retrieved weather metrics. This analysis helps identify potential trends or patterns in weather patterns across different geographical locations.

**Vacation Destination Recommendation:**

Based on the weather data analysis, the project aims to identify cities that might be ideal vacation destinations based on user-defined criteria.
Utilizing another API (details to be specified), the project retrieves information on hotels located near these ideal destinations.

**Output:**

The final outcome is a dataframe containing details on the recommended vacation cities and their corresponding nearby hotels. This dataframe can be visualized or further analyzed to aid users in making informed vacation decisions.

---------

## **Obtaining API Keys** ##
Before you are able to run the jupyter notebook files "WeatherPy" and "VacationPy" that are located inside the folder "WeatherPy" located on the main brach of this repository. You will need to obtain two API keys that are individual to your email address (these API keys that you obtain should be kept private and should only be known by you). The way to obtain the two API keys needed to run both the files metioned above is by going onto "https://www.geoapify.com/" and "https://openweathermap.org/api", and then creating a free account. You will then get an email from both of these websites saying to you need to activate your API keys and once that is completed, you will be able to use the API keys that they have provided for you. 

--------

## **WeatherPy Analysis** ##
There was a total of eight seperate scatter plots created using linear regression analysis to show the correlation between a given cities Latitude vs the metrics of Max Temp(C), Humidity(%), Cloudiness(%), and Wind Speed(m/s) based on if that given cities was located in the northern or southern hemisphere of the world.

**1) Latitude vs Max Temp(C) - Northern & Southern Hemisphere**

**Northern Hemisphere:**

![Lat_vs_Temp_NH](https://github.com/nmrodio/python-api-challenge/assets/157527614/c0ab2bd0-7595-42bf-9e4b-ebe2ea7af8c9)

**Southern Hemisphere:**

![Screenshot 2024-03-25 190916](https://github.com/nmrodio/python-api-challenge/assets/157527614/79a6710b-9309-4635-9759-07ee27d755cc)

*  As shown by linear regression lines plotted on the two graphs above regarding the correlation between the latitude of a given city vs the cities maximum temperature based on randomly generated cities located in both the northern hemisphere and southern hemisphere. The linear relationship between the latitude of cities in the northern hemisphere vs a cities maximum temperature has a moderately strong negative correlation which implies that as the given cities latitide is located more north (increase in latitude), the maximum temperature tends to decrease. This is also show by the linear regression line that predicts that the more north a city is located (increase in latitude), the cities maximum temperature tends to decrease. The linear relationship between the latitude of cities in the southern hemisphere vs a cities maximum temperature has a weak positive correlation which implies that as a given cities latitide is located more south (decrease in latitude), the maximum temperature tends to decrease. This is also shown by the linear regression line but since its a weak correlation, the line predicts that there might be a decrease in maximum temperature as a city is located more south. Although both of these scatter plots with their respective linear regression lines show a positive and negative relationship between a cities latitude vs maximum temperature in their respective hemipsheres, the common theme is that as a city is located closer to the equator (latitude = 0), the higher the maximum temperature of that city becomes. This makes sense because the equator receives the most amount of sunlight year round which would result in higher maximum temperatures and as a cities location gets futher away from the equator either north or south, the maxiumum tempteratures of cities will start to decrease.

**2) Latitude vs Humidity(%) - Northern & Southern Hemisphere**

**Northern Hemisphere:**

![Screenshot 2024-03-25 191357](https://github.com/nmrodio/python-api-challenge/assets/157527614/eb3ef5c6-7fdd-4c17-8614-dc4fb58e3956)

**Southern Hemisphere:**

![Screenshot 2024-03-25 191707](https://github.com/nmrodio/python-api-challenge/assets/157527614/2d3c806e-fae5-4e03-8284-5c2f804d66e2)

* As shown by linear regression lines plotted on the two graphs above regarding the correlation between the latitude of a given city vs the cities humidity based on randomly generated cities located in both the northern hemisphere and southern hemisphere. The linear relationship between the latitude of cities in the northern hemisphere vs a cities humidity has a weak positive correlation which implies that there is almost none to very little accociation between the two metrics of latitude vs humidity but the linear regression line does predict the more north a city is located (increase in latitude), there might be a very slight increase in humidity. The linear relationship between the latitude of cities in southern hemisphere vs a cities humidity has a very weak positive correlation, this implies that there is no association between a cities latitude vs its humidity in the southern hemisphere but the linear regression line does predict the more south a city is located (decrease in latitude), there might be a very slight increase in humidity. Although both of these scatter plots with their respective linear regression lines show a positive relationship between a cities latitude vs humidity in their respective hemipsheres, the correlations show that these metrics arent sufficent for explaining the cloudiness of a city based on a given cities latitude.

**3) Latitude vs Cloudiness(%) - Northern & Southern Hemisphere**

**Northern Hemisphere:**

![Screenshot 2024-03-25 191804](https://github.com/nmrodio/python-api-challenge/assets/157527614/71b90cf8-ceda-46c9-963e-d26dce82c2ce)

**Southern Hemisphere:**

![Screenshot 2024-03-25 191853](https://github.com/nmrodio/python-api-challenge/assets/157527614/e26f5caa-f015-429b-a937-eccf0dbe29f5)

* As shown by linear regression lines plotted on the two graphs above regarding the correlation between the latitude of a given city vs the cities cloudiness based on randomly generated cities located in both the northern hemisphere and southern hemisphere. The linear relationship between the latitude of cities in the northern hemisphere vs a cities cloudiness has a very weak positive correlation which implies that there is no association between the two metircs of latitude vs cloudiness but the linear regression line does predict the more north a city is located (increase in latitude), there might be a very slight increase in cloudiness. The linear relationship between the latitude of cities in southern hemisphere vs a cities cloudiness also has a very weak positive correlation, this implies that there is no association between a cities latitude vs its cloudiness in the southern hemisphere but the linear regression line does predict there might be a very slight increase in cloudiness as a cities is located more south (decrease in latitude). Although both of these scatter plots with their respective linear regression lines show a positive relationship between a cities latitude vs cloudiness in their respective hemipsheres, the correlations show that these metrics arent sufficent for explaining the cloudiness of a city based on a given cities latitude.

**4) Latitude vs Wind Speed(m/s) - Northern & Southern Hemisphere**

**Northern Hemisphere:**

![Screenshot 2024-03-25 191952](https://github.com/nmrodio/python-api-challenge/assets/157527614/934c1fd7-3cd7-4c3a-91c4-2f013e4a3706)

**Southern Hemisphere:**

![Screenshot 2024-03-25 192038](https://github.com/nmrodio/python-api-challenge/assets/157527614/11f2a0ba-7570-43c7-bd31-82d464646b0b)

* As shown by linear regression lines plotted on the two graphs above regarding the correlation between the latitude of a given city vs the cities wind speed based on randomly generated cities located in both the northern hemisphere and southern hemisphere. The linear relationship between the latitude of cities in the northern hemisphere vs a cities wind speed has a very weak negative correlation which implies that there is no association between the two metircs of latitude vs wind speed. The same can be seen by looking at the linear relationship between the latitude of cities in the southern hemisphere vs a cities wind speed, this relationship also has a very weak negative correlation which implies that there is no association between the two metircs of latitude vs wind speed. Although both of these scatter plots with their respective linear regression lines show a negative relationship between a cities latitude vs wind speed in their respective hemipsheres, the correlations show that these metrics arent sufficent for explaining the wind speed of a city based on a given cities latitude.
--------------
## **VacationPy Maps** ##

![Screenshot 2024-03-26 001257](https://github.com/nmrodio/python-api-challenge/assets/157527614/fc8f78f6-b4fb-43c3-b8a2-72b293bf4970)

![Screenshot 2024-03-26 001455](https://github.com/nmrodio/python-api-challenge/assets/157527614/4c62b6df-760f-4d9c-b72b-ad838c241bc6)

---------

## **How does the code work?** ##
**WeatherPy:**
1) Importing necessary dependencies to use later in the code (matplotlib, pandas, numpy, requests, time, scipy.stats / linregress, api_keys, citipy)
2) Creating an empty lists "lat_lngs" and "cities" to hold latitude and longitude combinations and cities names respectively => Defining the ranges for lat and long ==> Randomly finding 1500 combinations of lat and longs and then zipping them together to then find the nearest city using "citypy" and then appending the lat and long combinations to "lat_lngs" and cities to "cities" lists ===> Then printing out the number of cities in the "cities" list using len() function
3) Setting up base URL from "https://openweathermap.org/api" => Creating another empty list called "city_data" and then defining counters for the for loop
4) Start of for loop to loop through cities and then groups cities into "groups" of 50 for logging purposes
5) Setting up the endpoint URL to find the necessary metrics for each city and converting that data into .json() => Then pulling out only the citie metrics (latitude, longitude, max temp, humidity, cloudiness, wind speed, country, and date) from the list of dictionaries from the endpoint URL (There is a try and except compenent that allows the code to continue looping if a "nearest city" is NOT found from the API call)
6) Appending all the metrics mentioned above into the list "city_data" => Creating a dataframe called "city_data_df" from the data in "city_data" and then dislaying the record count and dataframe
7) Exporting the newly created dataframe into a CSV file called "cities.csv" to store the data that was pulled from the API request => Then reading that CSV file to allow for analysis purposes
8) Then four scatter plots are created to plot the points of a cities Latitude vs Max Temp(C), Humidity(%), Cloudiness(%), and Wind Speed(m/s) respectively => (The dates are converted from "UNIX-UTC" into a more readable format such as "Year-Month-Day")
9) A function called "linear_regress_hemis" is than created to create the linear regression line for the upcoming eight scatter plots and correlation is also calculated
10) A new smaller dataframe is created to only include cities that are located in the Northern Hemisphere (Latitude >= 0) and the same is done for Southern Hemisphere cities (Latitude <= 0)
11) The eight scatter plots are then created to show the correlation between a given cities Latitude vs the metrics of Max Temp(C), Humidity(%), Cloudiness(%), and Wind Speed(m/s) based on if that given cities was located in the northern or southern hemisphere of the world. (These are the screenshots that you see above)

**VacationPy:**
1) Importing necessary dependencies to use later in the code (hvplot.pands, pandas, requests, api_keys)
2) Reading the CSV file "cities.csv" that was created and saved from "WeatherPy" code => Then displaying the dataframe
3) Creating a map called "cities_worldwide_map" using hvplot.points using "Lng"                   # longitude of each city,
                                                                          "Lat"                 # Latitude of each city,
                                                                           geo = True             # Turns map into a geographic map,
                                                                           tiles = "OSM"         # Defines the "tiles" ==> OSM stands for "OpenStreetMap" which gives us the intuitive looking map below (white = land) &                                                                                                         (blue = water),
                                                                           size="Humidity"         # Makes the size of the plotted dots based on the humidity of each city where the nearest hotel is located,
                                                                           alpha = .5              # Alpha = .5 is making the colors of the dots more transparent so they arent so opaque making it easier to see where each                                                                                                       hotel is located on the map,
                                                                            color = "City"         # Assigning different colors for each city and puts the cities as a list/legend on the right side of the map,
                                                                            frame_width = 1000     # Makes the map output larger horizontally (width) so its easier to visualization,
                                                                            frame_height = 500      # Makes the map output larger vertically (height) so its easier to visualization

5) Displaying the map "cities_worldwide_map"
6) Creating a filtered dataframe called "specific_city_criteria_df" to narrow down cities to find ideal weather conditions for a vacation using the metrics of "Max Temp, "Wind Speed", and "Cloudiness" ==> Then adding the .dropna() function to drop all rows with null values to clean the dataframe
7) Creating a new dataframe called "hotel_df" with just the columns "City, Country, Lat, Lng , and Humidity" and then creating a copy using .copy() function => Then creating an empty column in the "hotel_df" dataframe called "Hotel Name" to be used for the API request in the next cell for storing the Hotel Names that are found using the API request from "https://www.geoapify.com/"
8) Next the radius and parameters where set to search for the nearest hotel - Params (categories, apiKey, and limit)
9) A for loop was then used to find the nearest hotel based on the lat and long of the ideal vacation cities from the "hotel_df" = Two other params were added (filter & bias to find the circle proximity based on the radius that was set above in the code)
10) The base URL was then define from "https://www.geoapify.com/" and then the end point URL was created by combining the params with the base URL to find the hotel names and then the data was converted into a .json() format - (There is a try and except compenent that allows the code to continue looping if a hotel is NOT found in the 10000 meter radius from the API call - if a hotel is not found for a given city in the "hotel_df" the code will print "No hotel found" in the "Hotel Name" column in the "hotel_df" dataframe)
11) A final map called "hotel_vacation_map" is then created using hvplot.points using "Lng"                                  # longitude of each city,
                                            "Lat"                                   # Latitude of each city,
                                            geo = True                              # Turns map into a geographic map,
                                            tiles = "OSM"                          # Defines the "tiles" ==> OSM stands for "OpenStreetMap" which gives us the intituve looking map below (white = land) & (blue = water),
                                            size="Humidity"                         # Makes the size of the plotted dots based on the humidity of each city where the nearest hotel is located,
                                            scale = 1.5                            # Scale = 1.5 is just increasing the size of the dots on the map for easier visualization,
                                            alpha = .5                              # Alpha = .5 is making the colors of the dots more transparent so they arent so opaque making it easier to see where each hotel is located on the map,
                                            color = "City"                          # Asigning different colors for each city and puts the cities as a list/legend on the right side of the map,
                                            hover_cols=["Hotel Name","Country"]     # Defines what other infomation that should be shown when you hover over a plot on the graph, 
                                            frame_width = 1000                      # Makes the map output larger horizontally (width) so its easier to visualization,
                                            frame_height = 500                     # Makes the map output larger vertically (height) so its easier to visualization

12) Displaying the map "hotel_vacation_map"

