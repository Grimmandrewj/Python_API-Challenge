## Goal
- I was tasked with analyzing data and generating plots to confirm quantitatively how the weather changes as one approaches and moves away from the equator.  
- I was given two challenges.  One (WeatherPy) to analyze the data and generate the plots to demonstrate the weather conditions by location.  The second (VacationPy), to plot cities that match my ideal weather conditions and find the nearest hotels within 10,000 meters.  

## Method
- For WeatherPy, random latitude and longitude coordinates were generated and names of cities matching the coordinates were logged using citipy. 
- The weather conditions were then logged for each city including max temperature, humidity, cloudiness, and wind speed.  
- These cities and their weather data were then displayed in a dataframe and written to a .csv file for further analysis.

![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/dd16158b-42c6-47ac-87f1-644ef9a7a44f)

- Scatter plots were then generated demonstrating city latitude vs. temperature, humidity, cloudiness, and wind speed.

![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/4314f190-82e4-4d05-9cda-2a9cde231a07)
![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/a6e30abf-1be2-4f8e-b294-332902ea1f35)
![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/5f26263d-a9c3-4e0d-a8c6-930c6cc74550)
![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/84e2a890-1041-45de-9ea0-97dd02c66ca5)

- The linear regression for each of the above relationships was then computed and displayed on the scatter charts

![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/0ef7e882-8a80-441f-b51f-53199ae95413)
![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/23738761-bdb1-4582-9872-7de40eb7c370)
![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/e1e35f92-04bf-40b8-bddd-fd1803c70d43)
![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/fc340d21-28da-464c-96a0-54a561891aca)

- For VacationPy, the .csv file created previously was then called and displayed in a dataframe

![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/604b7d4a-8334-462d-ae0a-b81f48135e2b)

- The hvplot module was utilized to plot a point for every city in the dataframe
- The dataframe was then limited to only the cities with the ideal weather conditions that I stipulated

![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/41d1b91f-f3e9-456b-8a3f-177795351397)

- From there, the geoapify module and API were used to find the nearest hotels within a 10,000 meter radius of the listed cities, and these results were displayed in a new dataframe.

![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/2f5ee57d-94ea-4cf4-a44f-ce39a8a540b4)

- These new hotel names were then added to the map as a hover message

![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/75e3d248-99c6-47d6-8ac3-0825241999d3)

![image](https://github.com/Grimmandrewj/Python_API_Challenge/assets/120341249/889fd2ab-6003-426f-aa26-94cb238eb227)



## Summary and Results
- The correlation between proximity to the equator and maximum temperature was confirmed to be a strong positive one.  However, the correlation between latitude and the other conditions were much weaker as demonstrated in the scatter plots.  
- The maps were successfully generated showing the closest hotels to the cities with the ideal weather conditions as required. 
