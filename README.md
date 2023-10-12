
# Weather Analysis

The repo contains 2 Jupyter Source Files WeatherPy.ipynb and VacationPy.ipynb which request relevant data from 2 API providers OpenWeatherMap and Geoapify for over 500 cities within the desired coordinates, and a repo output_data which contains the output images and a csv generated from WeatherPy.ipynb.

The two Jupyter Source Files utilize Pandas library to create DataFrame for each dataset. Matplotlib library was imported to create series of scatter plots based on different variables. Scipy and linregress were also imported to help with statistical computation and generate linear regresssion line for the data points. Citipy was imported to generate list of cities with the coordinates, hvplot was imported for interactive data visualization, and geoviews is imported to explore and visualize data geographically.
##  Resources


Tools : Python 3.7.6, Pandas, Jupyter Notebook

Python library: Matplotlib,Scipy, Citipy,hvplot

API: OpenWeatherMap and Geoapify 
## Instructions

There are two deliverables, WeatherPy and VacationPy.

### Part 1:WeatherPy

Create a Python script to visualize the weather of over 500 cities of varying distances from the equator

#### Requirement 1: 
Create Plots to Showcase the Relationship Between Weather Variables and Latitude.

Use the OpenWeatherMap API to retrieve weather data from the cities list generated using Citipy python library.

Create a series of scatter plots to showcase the following relationships:

Latitude vs. Temperature

Latitude vs. Humidity

Latitude vs. Cloudiness

Latitude vs. Wind Speed

#### Requirement 2:

Compute Linear Regression for Each Relationship.

Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). 

Create a series of scatter plotsand include the linear regression line, the model's formula, and the r values.

You should create the following plots:

Northern Hemisphere: Temperature vs. Latitude

Southern Hemisphere: Temperature vs. Latitude

Northern Hemisphere: Humidity vs. Latitude

Southern Hemisphere: Humidity vs. Latitude

Northern Hemisphere: Cloudiness vs. Latitude

Southern Hemisphere: Cloudiness vs. Latitude

Northern Hemisphere: Wind Speed vs. Latitude

Southern Hemisphere: Wind Speed vs. Latitude


### Part 2: VacationPy

Create a map that displays a point for every city from the csv file generated in Part 1.

Narrow down the data to find your ideal weather condition. For example:

A max temperature lower than 27 degrees but higher than 21

Wind speed less than 4.5 m/s

Zero cloudiness

For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

Add the hotel name and the country as additional information in the hover message for each city on the map.
## Results

### WeatherPy

#### Cities Data generated

![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/bd0ca6ea-5082-484e-84cc-2bd8510c63e3)

#### Latitude vs. Temperature
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/2d641bd0-aa7f-4941-b04b-cd9b5744e353)


#### Latitude vs. Humidity
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/e1382713-2d34-4e9f-819a-25faba1f3695)


#### Latitude vs. Cloudiness
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/7ffb6e96-4fa4-442d-bd77-4b64d3761af5)


#### Latitude vs. Wind Speed
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/2620a6ef-e621-49a0-8ed9-19d5121da6b8)


#### Northern Hemisphere: Temperature vs. Latitude
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/d60b8bc9-14db-4f8c-8632-8989bed9778a)

Northern Hemisphere cities show a strong negative correlation between latitude and temperature with a correlation coefficient of -0.8536412535831224.


#### Southern Hemisphere: Temperature vs. Latitude
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/89cfa6d1-d885-4d1f-97d0-fa04efd50939)

Southern Hemisphere cities show a weak postive correlation between latitude and temperature with a correlation coefficient of 0.1529383126859998.


#### Northern Hemisphere: Humidity vs. Latitude
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/25c42f69-6a09-4a69-af46-9eeb7768315e)

Northern Hemisphere cities show a weak positive correlation between humidity and temperature with a correlation coefficient of 0.1529383126859998.


#### Southern Hemisphere: Humidity vs. Latitude
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/7e26b077-0c00-416e-9a95-ff278d2a93c8)

Southern Hemisphere cities show a weak negative correlation between humidity and temperature with a correlation coefficient of -0.07388002463494117.



#### Northern Hemisphere: Cloudiness vs. Latitude
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/afdf2984-dee0-404e-88fa-33af3e648ee2)

Northern Hemisphere cities show a weak positive correlation between cloudiness and temperature with a correlation coefficient of 0.1782710377102286.


#### Southern Hemisphere: Cloudiness vs. Latitude
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/5522ddf9-7038-4e10-b7e5-ba7b9ed313e4)

Southern Hemisphere cities show a weak positive correlation between cloudiness and temperature with a correlation coefficient of 0.09154657701490135.



#### Northern Hemisphere: Wind Speed vs. Latitude
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/11aa4eab-2f50-45c8-b504-c6dd2a1fd299)

Northern Hemisphere cities show a weak positive correlation between Wind Speed and temperature with a correlation coefficient of 0.23834230327372638.

#### Southern Hemisphere: Wind Speed vs. Latitude
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/25755cd2-f051-4b4c-9046-4aed73404329)

Southern Hemisphere cities show a weak negative correlation between Wind Speed and temperature with a correlation coefficient of -0.06119779935026666.



### VacationPy

#### Map that displays a point for every city from the csv file generated in Part 1.
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/1bbd5e43-dc70-4ed2-8413-ceb9a021cda0)


#### Narrow down the data to find your ideal weather condition
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/9481f0d4-0e91-41c2-80f6-6e35a765a793)


#### For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/e11e8cfe-31ee-4efd-b54f-d09c42c0a33f)



#### Hotel name and the country as additional information in the hover message for each city on the map.
![image](https://github.com/ShubhangiBidkar/python-api-challenge/assets/38162670/2763f9f4-143a-445a-8e43-7e69f1c8bc7a)
