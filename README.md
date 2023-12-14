# Final-Project-Statistical-Modelling-with-Python

## Project/Goals
To query the API and understand data returned from my city of choice from the API. Compare the quality of the Yelp and Foursquare API in terms of quality of information they both give, use data visualization to explore the data, and then create a SQLite database and store the data you've collected on the POIs. Validate the data and finally build a regression model that demonstrates a relationship between the number of bikes in a particular location and the characteristics of the POIs in that location, using Python’s `statsmodels` module.


## Process

The process were as follows:
1. Explore the structure of the API, query the API and understand the data returned. 
2. Choose a city covered by the CityBikes API and retrieve all available bike stations in that city. 
3. For each bike station, use the API to call the latitude, longitude and number of bikes. 
4. Parse the JSON object into a Pandas dataframe. 
5. Connect to the  [Foursquare](https://developer.foursquare.com/places) API
6. Connect to the [Yelp](https://www.yelp.com/developers/documentation/v3/get_started) API. This API offers similar services as Foursquare.
7. For each of the bike stations in Part 1, query both APIs to retrieve information for the following in that location:
 - Restaurants or bars
 - Various POIs (points of interest) of your choice
8. Create a DataFrame for the Yelp results and Foursquare results. 
9. Compare the quality of the Yelp and Foursquare API. For your location, which API gives you the most complete information/better coverage?
10. Join the data from Part 1 with the data from Part 2 to create a new dataframe. 
11. Use data visualization to explore the data. 
12. Create your own SQLite database and store the data you've collected on the POIs. **Put some thought into the structure of your database.** We've used and created sqlite3 databases before in the activity [**SQL in Python**](https://data.compass.lighthouselabs.ca/b9e08cd5-68c6-490c-a32b-a66f01bf53e1).
13. Validate your data.
14. Build a regression model using Python’s `statsmodels` module that demonstrates a relationship between the number of bikes in a particular location and the characteristics of the POIs in that location.  
15. Interpret results. Expand on the model output, and derive insights from your model.


## Results
I realised, for my chosen city, the YELP API gave me better and more information than the Foursquare API.

## Challenges 
1. There was a daily limit to the amount of times one could query the YELP database. I had a limit of 500 daily.
2. I spent a lot of time with picking the right city, as some cities either did not have enough bike stations, or had too many.

## Future Goals
1. I would have perfected the Model and actually ran codes to turn it from a regression problem into a classification one.



Please note; I have also attached 5 csv files ("df_Yelp.csv", "foursquare_info.csv", "merged_df.csv", "new_Yelp.csv", "station_info.csv") from each python file. I had to read them to use them in the subsequent files. It saved me time.