# PythonWeatherapp
This Python application fetches weather data using the OpenWeatherMap API and provides current weather conditions as well as a 5-day forecast for a specified location (city).

Requirements
Python 3.x
requests library
OpenWeatherMap API key
Installation
Install Python from the official website: Python.org
Install the requests library using pip:
pip install requests
Usage
Obtain an API key from OpenWeatherMap by signing up at OpenWeatherMap.org and subscribing to their API services.
Replace "YOUR_API_KEY" in the code with your actual API key obtained from OpenWeatherMap.
Run the Python script weather.py.
Enter the name of the city for which you want to fetch weather data when prompted.
Code Structure
fetch_current_weather(city, api_key): Function to fetch current weather data for a specified city using the OpenWeatherMap API.
fetch_5_day_forecast(city, api_key): Function to fetch the 5-day weather forecast for a specified city using the OpenWeatherMap API.
display_current_weather(weather_data): Function to display current weather conditions including temperature, weather description, humidity, wind speed, sunrise time, and sunset time.
display_5_day_forecast(forecast_data): Function to display the 5-day weather forecast including daily temperature and weather conditions.
main(): Main function to execute the program. Prompts the user to enter a city name, fetches weather data, and displays it.
External Dependencies
requests: Used to make HTTP requests to the OpenWeatherMap API.
datetime: Used to handle date and time operations, particularly in formatting timestamps.
API Usage
OpenWeatherMap API: The application interacts with the OpenWeatherMap API to fetch weather data. It uses two endpoints:
Current Weather Data: Retrieves current weather data for a specified city.
5 Day Weather Forecast: Retrieves the 5-day weather forecast for a specified city.
Error Handling
If the city entered by the user is not found in the API database, the program displays a "City not found" error message and prompts the user to try again.
If there are any issues with fetching weather data from the API or parsing the response, appropriate error messages are displayed.
