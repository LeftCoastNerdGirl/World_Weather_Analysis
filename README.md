# Analyzing API weather data

The first challenge involves using an API key to pull data from open weather map dot org and using it to analyze weather patterns based on latitude.  

Once the data is extracted and cleaned, it is stored in a Pandas dataframe. That data is then exported to a csv file.  The dataframe is then used in conjunction with Matplotlib to create scatterplots displaying the following relationships:  

Latitude vs. Temperature  
Latitude vs. Humidity  
Latitude vs. Cloudiness  
Latitude vs. Wind Speed  

![image](https://github.com/user-attachments/assets/e555fa67-0019-4ef3-ba77-a51abf322111)


Next, using Scipy stats library, r-squared is calculated and linear regression lines plotted to analyze the correlations between the various weather elements and the latitude of the areas tested. The following plots were created and analysis explained:

Northern Hemisphere: Temperature vs. Latitude    
Southern Hemisphere: Temperature vs. Latitude  
Northern Hemisphere: Humidity vs. Latitude  
Southern Hemisphere: Humidity vs. Latitude  
Northern Hemisphere: Cloudiness vs. Latitude  
Southern Hemisphere: Cloudiness vs. Latitude  
Northern Hemisphere: Wind Speed vs. Latitude  
Southern Hemisphere: Wind Speed vs. Latitude  

![image](https://github.com/user-attachments/assets/43228f05-b6d8-4587-80db-2b1968f13b2c)


![image](https://github.com/user-attachments/assets/03626dc3-ffe2-41c1-a122-4de7a5c310be)


The second challenge for this project imports the city output data file from challenge 1 and uses various datapoints to create maps and information to help plan an upcoming vacation.  

Using hvplot from Pandas and geodata imported from Geoapify via API, map visualizations are created.  

The cities are mapped with points sized based on humidity:  

![image](https://github.com/user-attachments/assets/7cc8ddb3-22fc-4483-9687-34725d0cce03)


The next step is to limit the weather data based on temperature - lower than 27ºC degrees but higher than 21ºC. This reduced dataframe was then matched with a dataframe containing a list of hotels with their longitude and latitude. The purpose of this comparison was to find the hotel nearest to the ideal weather conditions we'd created.  

The combined dataframe, with weather conditions based on the temperature filter with the nearest hotels was then mapped, with humidity again indicated by the size of the plot point. The resulting map shows our ideal vacation locations! 


![image](https://github.com/user-attachments/assets/ff947ebd-5042-4161-9958-8daf0c475648)
