
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

#### Latitude vs. Temperature

#### Latitude vs. Humidity

#### Latitude vs. Cloudiness

#### Latitude vs. Wind Speed

#### Northern Hemisphere: Temperature vs. Latitude

#### Southern Hemisphere: Temperature vs. Latitude

#### Northern Hemisphere: Humidity vs. Latitude

#### Southern Hemisphere: Humidity vs. Latitude

#### Northern Hemisphere: Cloudiness vs. Latitude

#### Southern Hemisphere: Cloudiness vs. Latitude

#### Northern Hemisphere: Wind Speed vs. Latitude

#### Southern Hemisphere: Wind Speed vs. Latitude


### VacationPy

#### Map that displays a point for every city from the csv file generated in Part 1.

#### Narrow down the data to find your ideal weather condition

#### For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.

#### Hotel name and the country as additional information in the hover message for each city on the map.