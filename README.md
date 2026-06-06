# Weather Forecast

A lightweight weather application built with HTML, CSS, and vanilla JavaScript. It uses the browser's geolocation API to display current weather conditions for the user's location.

## Features

- Current temperature and weather conditions
- Location-based forecast using browser geolocation
- Celsius and Fahrenheit temperature toggle
- Weather icons for daytime and nighttime conditions
- Responsive, dependency-free interface

## Run Locally

Geolocation works on `localhost` or over HTTPS. Start a local web server from the project directory:

```bash
python3 -m http.server 8000
```

Then open [http://localhost:8000](http://localhost:8000) and allow location access when prompted.

## Configuration

The app retrieves weather data from [OpenWeatherMap](https://openweathermap.org/). Set a valid API key in `app.js` before running the project:

```js
const key = "YOUR_OPENWEATHERMAP_API_KEY";
```

For a production deployment, route API requests through a backend or serverless function instead of exposing the key in client-side code.

## Project Structure

```text
.
├── app.js        # Geolocation, weather requests, and UI updates
├── index.html    # Application markup
├── style.css     # Layout and visual styles
├── font/         # Local font files
└── icons/        # Weather condition icons
```

## Credits

Weather data is provided by [OpenWeatherMap](https://openweathermap.org/).

Weather icons are based on the [Weather Underground Icons](https://github.com/manifestinteractive/weather-underground-icons) collection by Ashley Jager.
