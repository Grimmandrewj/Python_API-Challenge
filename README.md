## Goal
- I was tasked with analyzing data and generating plots to confirm quantitatively how the weather changes as one approaches and moves away from the equator.  
- I was given two challenges.  One (WeatherPy) to analyze the data and generate the plots to demonstrate the weather conditions by location.  The second (VacationPy), to plot cities that match my ideal weather conditions and find the nearest hotels within 10,000 meters.  

## Method
- For WeatherPy, random latitude and longitude coordinates were generated and names of cities matching the coordinates were logged using citipy. 
- The weather conditions were then logged for each city including max temperature, humidity, cloudiness, and wind speed.  
- These cities and their weather data were then displayed in a dataframe and written to a .csv file for further analysis. 
- Scatter plots were then generated demonstrating city latitude vs. temperature, humidity, cloudiness, and wind speed. 
- The linear regression for each of the above relationships was then computed and displayed on the scatter charts
- For VacationPy, the .csv file created previously was then called and displayed in a dataframe
- The hvplot module was utilized to plot a point for every city in the dataframe
- The dataframe was then limited to only the cities with the ideal weather conditions that I stipulated
- From there, the geoapify module and API were used to find the nearest hotels within a 10,000 meter radius of the listed cities, and these results were displayed in a new dataframe.  
- These new hotel names were then added to the map as a hover message 

## Results
- The correlation between proximity to the equator and maximum temperature was confirmed to be a strong positive one.  However, the correlation between latitude and the other conditions were much weaker as demonstrated in the scatter plots.  
- The maps were successfully generated showing the closest hotels to the cities with the ideal weather conditions as required. 
