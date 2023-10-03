# Python-API-Challenge
 
**Instructions

This activity is broken down into two deliverables, WeatherPy and
VacationPy. In this deliverable, you'll create a Python script to visualize
the weather of over 500 cities of varying distances from the equator.

**Part 1: WeatherPy

To get started, the code required to generate random geographic coordinates and the nearest city to each latitude and longitude combination is provided.

**Requirement 1: Create Plots to Showcase the Relationship Between Weather Variables and Latitude

To fulfill the first requirement, you'll use the OpenWeatherMap API to retrieve weather data from the cities list generated in the starter code. Next, you'll create a series of scatter plots to showcase the following relationships:
        1.Latitude vs. Temperature
        2.Latitude vs. Humidity
        3.Latitude vs. Cloudiness
        4.Latitude vs. Wind Speed
        
**Requirement 2: Compute Linear Regression for Each Relationship

To fulfill the second requirement, compute the linear regression for each relationship. Separate the plots into Northern Hemisphere (greater than or equal to 0 degrees latitude) and Southern Hemisphere (less than 0 degrees latitude). You may find it helpful to define a function in order to create the linear regression plots.

Next, create a series of scatter plots. Be sure to include the linear regression line, the model's formula, and the r values as you can see in the following image
 
You should create the following plots:

    1.Northern Hemisphere: Temperature vs. Latitude
    2.Southern Hemisphere: Temperature vs. Latitude
    3.Northern Hemisphere: Humidity vs. Latitude
    4.Southern Hemisphere: Humidity vs. Latitude
    5.Northern Hemisphere: Cloudiness vs. Latitude
    6.Southern Hemisphere: Cloudiness vs. Latitude
    7.Northern Hemisphere: Wind Speed vs. Latitude
    8.Southern Hemisphere: Wind Speed vs. Latitude
    
After each pair of plots, explain what the linear regression is modeling. Describe any relationships that you notice and any other findings you may uncover.

**Part 2: VacationPy

In this deliverable, you'll use your weather data skills to plan future vacations. Also, you'll use Jupyter notebooks, the geoViews Python library, and the Geoapify API.

The code needed to import the required libraries and load the CSV file with the weather and coordinates data for each city created in Part 1 is provided to help you get started.

Your main tasks will be to use the Geoapify API and the geoViews Python library and employ your Python skills to create map visualizations.

To succeed on this deliverable of the assignment, open the VacationPy.ipynb starter code and complete the following steps:

        1.Create a map that displays a point for every city in the city_data_df DataFrame as shown in the following image. The size of the point should be the humidity in each city.

        2.Narrow down the city_data_df DataFrame to find your ideal weather condition. For example:
            A max temperature lower than 27 degrees but higher than 21
            Wind speed less than 4.5 m/s
            Zero cloudiness
                NOTE:Feel free to adjust your specifications but make sure to set a reasonable limit to the number of rows returned by your API requests.

        3.Create a new DataFrame called hotel_df to store the city, country, coordinates, and humidity.
        4.For each city, use the Geoapify API to find the first hotel located within 10,000 meters of your coordinates.
        5.Add the hotel name and the country as additional information in the hover message for each city on the map as in the following image:

**Hints and Considerations

1.The city data that you generate is based on random coordinates and different query times, so your outputs will not be an exact match to the provided starter notebook.

2.If you'd like a refresher on the geographic coordinate system, this siteLinks to an external site. has great information.

3.Take some time to study the OpenWeatherMap API. Based on your initial study, you should be able to answer basic questions about the API: Where do you request the API key? Which Weather API in particular will you need? What URL endpoints does it expect? What JSON structure does it respond with? Before you write a line of code, you should have a crystal-clear understanding of your intended outcome.

4.A starter code for citipy has been provided. However, if you're craving an extra challenge, push yourself to learn how it works by using the citipy Python libraryLinks to an external site.. Before you try to incorporate the library in your analysis, start with simple test cases outside of your main script to confirm that you are using it correctly. Often, when introduced to a new library, learners spend hours trying to figure out errors in their code when a simple test case can save you a lot of time and frustration.

5.You will need to apply your critical thinking skills to understand how and why we're recommending these tools. What is citipy used for? Why would you use it in conjunction with the OpenWeatherMap API? How would you do so?

6.While building your script, pay attention to the cities you are using in your query pool. Are you covering the full range of latitudes and longitudes? Or are you choosing 500 cities from one region of the world? Even if you were a geography genius, simply listing 500 cities based on your personal selection would create a biased dataset. Try to think of ways that you can counter these selection issues.

        a.    Hint: Consider the full range of latitudes.
        
7.Once you have computed the linear regression for one relationship, you will follow a similar process for all other charts. Optionally, try to create a function that will create these charts based on different parameters. (Note: there will be no extra points for completing this.)

8.Remember that each coordinate will trigger a separate call to the Google API. If you're creating your own criteria to plan your vacation, try to reduce the results in your DataFrame to 10 or fewer cities.

9.Ensure that your repository has regular commits and a thorough README.md file.

10. Lastly, remember that this is a challenging activity. Push yourself! If you complete this task, you can safely say that you've gained a strong understanding of the core foundations of data analytics, and it will only get better from here.



<img src="/Users/dalyalami/Desktop/Screen Shot 2023-10-02 at 10.35.33 PM.png" alt="Alt text"