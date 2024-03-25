# **python-api-challenge** #
--------

## Obtaining API Keys
* Before you are able to run the jupyter notebook files "WeatherPy" and "VacationPy" that are located inside the folder "WeatherPy" located on the main brach of this repository. You will need to obtain two API keys that are individual to your email address (these API keys that you obtain should be kept private and should only be known by you). The way to obtain the two API keys needed to run both the files metioned above is by going onto "https://www.geoapify.com/" and "https://openweathermap.org/api", and then creating a free account. You will then get an email from both of these websites saying to you need to activate your API keys and once that is completed, you will be able to use the API keys that they have provided for you. 
--------

## WeatherPy Analysis
There was a total of eight seperate scatter plots created using linear regression analysis to show the correlation between a given cities Latitude vs the metrics of Max Temp(C), Humidity(%), Cloudiness(%), and Wind Speed(m/s) based on if that given cities was located in the northern or southern hemisphere of the world.

1) Latitude vs Max Temp(C) - Northern & Southern Hemisphere

Northern Hemisphere
![image]

Southern Hemisphere 
PUT SCREENSHOT HERE

*  As shown by linear regression lines plotted on the two graphs above regarding the correlation between the latitude of a given city vs the cities maximum temperature based on randomly generated cities located in both the northern hemisphere and southern hemisphere. The linear relationship between the latitude of cities in the northern hemisphere vs a cities maximum temperature has a moderately strong negative correlation which implies that as the given cities latitide is located more north (increase in latitude), the maximum temperature tends to decrease. This is also show by the linear regression line that predicts that the more north a city is located (increase in latitude), the cities maximum temperature tends to decrease. The linear relationship between the latitude of cities in the southern hemisphere vs a cities maximum temperature has a weak positive correlation which implies that as a given cities latitide is located more south (decrease in latitude), the maximum temperature tends to decrease. This is also shown by the linear regression line but since its a weak correlation, the line predicts that there might be a decrease in maximum temperature as a city is located more south. Although both of these scatter plots with their respective linear regression lines show a positive and negative relationship between a cities latitude vs maximum temperature in their respective hemipsheres, the common theme is that as a city is located closer to the equator (latitude = 0), the higher the maximum temperature of that city becomes. This makes sense because the equator receives the most amount of sunlight year round which would result in higher maximum temperatures and as a cities location gets futher away from the equator either north or south, the maxiumum tempteratures of cities will start to decrease.

2) Latitude vs Humidity(%) - Northern & Southern Hemisphere

Northern Hemisphere
PUT SCREENSHOT HERE

Southern Hemisphere
PUT SCREENSHOT HERE

* As shown by linear regression lines plotted on the two graphs above regarding the correlation between the latitude of a given city vs the cities humidity based on randomly generated cities located in both the northern hemisphere and southern hemisphere. The linear relationship between the latitude of cities in the northern hemisphere vs a cities humidity has a weak positive correlation which implies that there is almost none to very little accociation between the two metrics of latitude vs humidity but the linear regression line does predict the more north a city is located (increase in latitude), there might be a very slight increase in humidity. The linear relationship between the latitude of cities in southern hemisphere vs a cities humidity has a very weak positive correlation, this implies that there is no association between a cities latitude vs its humidity in the southern hemisphere but the linear regression line does predict the more south a city is located (decrease in latitude), there might be a very slight increase in humidity. Although both of these scatter plots with their respective linear regression lines show a positive relationship between a cities latitude vs humidity in their respective hemipsheres, the correlations show that these metrics arent sufficent for explaining the cloudiness of a city based on a given cities latitude.

3) Latitude vs Cloudiness(%) - Northern & Southern Hemisphere

Northern Hemisphere
PUT SCREENSHOT HERE

Southern Hemisphere
PUT SCREENSHOT HERE

* As shown by linear regression lines plotted on the two graphs above regarding the correlation between the latitude of a given city vs the cities cloudiness based on randomly generated cities located in both the northern hemisphere and southern hemisphere. The linear relationship between the latitude of cities in the northern hemisphere vs a cities cloudiness has a very weak positive correlation which implies that there is no association between the two metircs of latitude vs cloudiness but the linear regression line does predict the more north a city is located (increase in latitude), there might be a very slight increase in cloudiness. The linear relationship between the latitude of cities in southern hemisphere vs a cities cloudiness also has a very weak positive correlation, this implies that there is no association between a cities latitude vs its cloudiness in the southern hemisphere but the linear regression line does predict there might be a very slight increase in cloudiness as a cities is located more south (decrease in latitude). Although both of these scatter plots with their respective linear regression lines show a positive relationship between a cities latitude vs cloudiness in their respective hemipsheres, the correlations show that these metrics arent sufficent for explaining the cloudiness of a city based on a given cities latitude.

4) Latitude vs Wind Speed(m/s) - Northern & Southern Hemisphere

Northern Hemisphere
PUT SCREENSHOT HERE

Southern Hemisphere
PUT SCREENSHOT HERE

* As shown by linear regression lines plotted on the two graphs above regarding the correlation between the latitude of a given city vs the cities wind speed based on randomly generated cities located in both the northern hemisphere and southern hemisphere. The linear relationship between the latitude of cities in the northern hemisphere vs a cities wind speed has a very weak negative correlation which implies that there is no association between the two metircs of latitude vs wind speed. The same can be seen by looking at the linear relationship between the latitude of cities in the southern hemisphere vs a cities wind speed, this relationship also has a very weak negative correlation which implies that there is no association between the two metircs of latitude vs wind speed. Although both of these scatter plots with their respective linear regression lines show a negative relationship between a cities latitude vs wind speed in their respective hemipsheres, the correlations show that these metrics arent sufficent for explaining the wind speed of a city based on a given cities latitude. 
