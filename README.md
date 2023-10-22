# Weather-Api
The script fetches the current weather data for a specified city using the OpenWeatherMap API and displays details such as temperature, humidity, wind speed, and sunrise/sunset timings.

## Weather Fetcher: README

### Introduction:
This script fetches the current weather data for a specified city using the OpenWeatherMap API.

### Requirements:

1. Python 3.x
2. Python libraries:
   - `requests`: For sending HTTP requests.
   - `datetime`: To handle date and time related tasks.

### Setup:

1. Make sure you have the required libraries installed:
   ```
   pip install requests
   ```

2. An API key from OpenWeatherMap is required to use their service. In the code provided, a sample API key is given with the variable name `API_KEY`. However, it's recommended to get your own API key by registering on the OpenWeatherMap website.

### Usage:

1. Run the script:
   ```
   python weather_fetcher.py
   ```

2. You'll be prompted to enter the name of the city for which you want to fetch the weather information.

3. Once you provide the city's name, the script will fetch and display the following weather details:
   - Temperature in Celsius and Fahrenheit
   - "Feels Like" temperature in Celsius and Fahrenheit
   - Humidity percentage
   - Wind speed in m/s
   - General weather description (e.g., clear sky, rain, etc.)
   - Local sunrise and sunset time

### Functions:

1. `kelvin_to_celcius_fahrenheit(kelvin)`: This function takes temperature in Kelvin and returns its equivalent in Celsius and Fahrenheit.

### Notes:

- Ensure your API key is valid and has the necessary permissions to access the desired data.
- API calls might be rate-limited. Consider implementing error handling or retry mechanisms if required.
- The script fetches data in real-time, so every time you run the script, you might see different values based on the current weather conditions.
- As the OpenWeatherMap API provides temperature in Kelvin by default, the script includes a function to convert it to more commonly used Celsius and Fahrenheit.

### Disclaimer:
Always refer to OpenWeatherMap's terms of service when using their API, especially for production or commercial use. The provided API key in the script is for demonstration purposes and might not work due to usage restrictions or expiry. Always obtain your own API key from OpenWeatherMap's official website.
