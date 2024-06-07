# Weather App Using Java in Android

This project involves creating an Android Weather App using Java. The weather information is retrieved using the [OpenWeatherMap](https://openweathermap.org) API, which provides data such as temperature, pressure, humidity, weather conditions, and the times of sunrise and sunset.

## Obtaining an API Key from OpenWeatherMap

To retrieve weather data, we use the **OpenWeatherAPI**, which requires an API key. Follow the steps below to obtain your API key:

1. Create a new account [here](https://home.openweathermap.org/users/sign_up).
2. After logging in, go to the API keys section [here](https://home.openweathermap.org/api_keys) to get your API key.

## Fetching Weather Information Using Latitude & Longitude

To request weather information based on the **latitude** and **longitude** of a location, use the following code:

```java
String response = HttpRequest.executeGet("https://api.openweathermap.org/data/2.5/weather?lat=" + LAT + "&lon=" + LON + "&units=metric&appid=" + API_KEY);
```

Here, LAT and LON represent the latitude and longitude, respectively. To display weather information for the user's current location, you need to detect the current latitude and longitude. 
