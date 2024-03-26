# python-api-challenge

The purpose of this analysis is to answer the following question using tools such as Python, JSON, and API: What is the weather like as we approach the equator?

## Tools needed to become an expert in weather analysis:

* Create a new repository named python-api-challenge for this project.

* Clone the newly created repository to your local computer.

* Within your local Git repository, establish a directory dedicated to this assignment, naming it in accordance with the Challenges, e.g., WeatherPy.

* Inside the designated folder, incorporate the provided files api_keys.py, WeatherPy.ipynb, and  VacationPy.ipynb from the starter code ZIP file.

* Before pushing your modifications to GitHub, include a .gitignore file.

* Module 6 files

## Add a .gitignore file

* Create a .gitignore file to safeguard the API key in api_keys.py from public exposure on GitHub.

* Check the list of untracked files by typing git status in the command line.

* To add specific files, like WeatherPy.ipynb, to GitHub, use the command git add WeatherPy.ipynb.

* For a more efficient approach, include all files you don't want to track in the .gitignore file.

* Add api_keys.py to the .gitignore file by opening the python-api-challenge folder in VS Code, then inserting "# Adding config.py file." followed by "api_keys.py" on the first line of the .gitignore file.

* Verify the modification of the .gitignore file and the untracked status of api_keys.py by typing git status in the command line.

* Utilize git add, git commit, and git push commands to commit the modifications to the .gitignore, WeatherPy.ipynb, and VacationPy.ipynb files to GitHub.

* Upon inspection on GitHub, only WeatherPy.ipynb and VacationPy.ipynb files should be visible as new python files.
    
# Part 1: WeatherPy

Task: Create a Python script to visualize weather data from over 500 cities at varying distances from the equator.
    
Tools: Utilize the citipy Python library and the OpenWeatherMap API.

Approach: Employ problem-solving skills to model weather patterns across cities.

   -Use the provided WeatherPy.ipynb Jupyter notebook in the starter code ZIP file.
    
   -The starter code includes functionality for generating random geographic coordinates and determining the nearest city for each latitude and longitude combination.
    
   ## Requirement 1
* Retrieve weather data from the cities list generated in the starter code using the OpenWeatherMap API.

* Create scatter plots to demonstrate the relationships between latitude and the following weather variables:
  - Temperature
       
  - Humidity
        
  - Cloudiness
        
  - Wind Speed
  ## Requirement 2      
* Compute linear regression for each relationship between latitude and weather variables.

* Divide plots into Northern Hemisphere (≥ 0° latitude) and Southern Hemisphere (< 0° latitude).

* Define a function to facilitate creation of linear regression plots.

* Generate scatter plots for the following pairs, including linear regression lines, model formulas, and r values:

   - Northern Hemisphere: Temperature vs. Latitude
   
   - Southern Hemisphere: Temperature vs. Latitude
   
   - Northern Hemisphere: Humidity vs. Latitude
   
   - Southern Hemisphere: Humidity vs. Latitude
   
   - Northern Hemisphere: Cloudiness vs. Latitude
   
   - Southern Hemisphere: Cloudiness vs. Latitude
   
   - Northern Hemisphere: Wind Speed vs. Latitude
   
   - Southern Hemisphere: Wind Speed vs. Latitude
        
* Analyze each pair of plots, discussing the modeling of linear regression, observed relationships, and any noteworthy findings.
    
# Part 2: VacationPy

* Utilize Jupyter notebooks, the geoViews Python library, and the Geoapify API to plan future vacations based on weather data.
   
* Import necessary libraries and load the CSV file containing weather and coordinates data for each city from Part 1.

* Create a map displaying a point for each city in the city_data_df DataFrame, with the size of the point indicating the humidity in each city.
    
* Narrow down the city_data_df DataFrame to identify ideal weather conditions, such as:
    * Maximum temperature lower than 27°C but higher than 21°C
         
    * Wind speed less than 4.5 m/s
         
    * Cloudiness of zero
    
* Implement these steps in the VacationPy.ipynb starter code and visualize the resulting map with humidity-based point sizes.