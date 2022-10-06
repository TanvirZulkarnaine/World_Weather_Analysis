# World_Weather_Analysis

## Overview of this project
This project consists of three parts, Weather_Database, Vacation_Search, and Vacation_Itinerary. 

### Deliverable 1: Weather_Database
For this part of the project is that I create 2000 random latitude and longitude pair of tuples and storing them in a list. Using the lats and long coordinates, I collected a list of cities using cityPy module. Then I used open weather map's API key to collect information of the weather of the city and stored them in a list. This process took a while. With the data collected using open weather map's api, I stored the data in a dataframe and exported the dataframe in a csv file. 

### Deliverable 2: Vacation_Search
I imported the previously saved csv file as a dataframe. I filtered the dataframe according to a range of suitable temperature according to user's choice and store the data in a new dataframe. I added a new empty column in my dataframe that is called Hotel name. I used google's api key to collect all the hotel information according to the longitude and latitude in the dataframe and filled up my hotel name column with hotels. Some hotels were not find given latitude and longitudes, thus I had to delete the rows which could not collect hotel names. I saved this new dataframe as WeatherPy_vacation.csv. I created a html script that holds the information of the city/weather/max temp, and using gmaps, I displayed the hotel locations with their respective information. 

### Deliverable 3: Vacation_Itinerary
Again, I imported the google api key, and other necessary imports. I also imported WeatherPy_vacation.csv file into a dataframe. Next, same as deliverable 2, I displayed the gmaps figure with the info box. For the next part, I created four dataframes by filtering the imported dataframe and these four dataframe holds information about one city for each. I made sure that these cities are in the same countries. I stored the lats and long pairs of these cities into variables nameed stop #1-3. Then I used google's directional layer map and displayed a circular path that describes the customer's travel route from start to finish and it accounts fot their stops. Lastly, I usied gmaps figure to display the information of these four cities. 
