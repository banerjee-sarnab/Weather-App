### Weather App

This is a weather browsing application using the OpenWeatherMap API and GeoDB API with places autocomplete, along with various React JS skills.

### Features

- Display current weather information including temperature, humidity, and weather condition.
- Search for weather information by location.
- Automatically detects and displays weather for the user's current location.
- Displays the forecast for the seven days of the queried location
- User-friendly and responsive design.


## Getting Started

To run the Weather App locally, follow these steps:

1. Clone this repository:

   ```bash
   git clone https://github.com/banerjee-sarnab/Weather-App.git
   ```

2. Navigate to the project directory:

   ```bash
   cd weather-app
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Obtain an API key from OpenWeather. Replace `YOUR_OPENWEATHER_API_KEY` in the `src/App.js` file with your API key.

5. Start the development server:

   ```bash
   npm start
   ```

6. Open your web browser and visit `http://localhost:3000` to use the Weather App.

## Usage

- Upon opening the Weather App, the current weather for your location will be displayed automatically if you grant location access.
- To manually search for weather in a different location, use the search bar and click the search button.

## Technologies Used

- React.js
- OpenWeather API
- GeoDB API
- HTML5 and CSS3

## Credits

- Weather data provided by [OpenWeather](https://openweathermap.org/).
- Location search powered by [GeoDB](https://geodb.dev/).

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
