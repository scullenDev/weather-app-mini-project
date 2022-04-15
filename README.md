# Geocoding and Weather API Challenge

## Getting Started:

1. Make a copy of the prior demo as your starter code. (You can optionally choose to create a new `create-react-app` app to work from.)
2. Within your team, appoint at least one person to register a free API key at [OpenWeatherMap.org](https://openweathermap.org/price).
3. In the root directory of your React app (*NOT* within `/src`) create a file called `.env`. Within this file, paste the following line of code:

```
REACT_APP_API_KEY=yourkeygoeshere
```

4. Make sure to replace 'yourkeygoeshere' with the key you received from the API. Then save the `.env` file and restart your React server.
5. Study the starter code and the app's functionality and discuss it with your teammates; make sure each of you has a good understanding of how the code works.

---

## Ideas for Improvements:

1. **(recommended)** Create a simple form with an input field and a submit button. Then wire the form up so that the input reads from/writes to the existing state variable of 'location' (a controlled form). On submission of the form, run a geocode and a weather search using the existing APIs to get weather data for this new location and load it into state. Be sure to DRY your code and use methods where possible to avoid repeated code!
2. **(recommended)** Rewrite the component so that rather than displaying the JSON data received from the weather API, your app shows the current forecast in a neat and easy-to-understand way.
3. **(recommended)** Put a real loading spinner in in place of the text 'Pretend I'm a loading spinner!!!'
4. Reference the API's [Weather Icons Documentation](https://openweathermap.org/weather-conditions) and use this functionality to show the appropriate icon within your current weather forecast display.
5. Research how you can request a user's location via the web browser. When present, use this location as the default 'location' state instead of 'Fresno, CA'. Note: you may need to modify your API calls in this case, as this technique will likely give you access to a latitude/longitude initially with no need to geocode. How can you make your API calls flexible enough to work with any type of location (lat/lng, zip code, city and state, landmark, etc)?
6. Refactor the starter code to use either chained promises or `async/await`.
7. Divide your app into multiple reusable components.
8. Refactor the code to use Fetch rather than axios, or to use a different free geocoding and/or weather API.
9. Use destructuring where possible to simplify your code's readability.
10. Implement defensive code within you axios `.then()` blocks to do an 'early return' if the user's input value is invalid. (For an example of this behavior, set the 'location' state's initial value to an empty string and check the console for an error!)
11. Research the docs for the [OpenWeatherMap.org APIs](https://openweathermap.org/api) and implement additional functionality of your choice.
12. Refactor your app's code to use an uncontrolled form and input for collecting the user's location. Use `useRef()` to access and update the value.
