# Weather App

_A simple and intuitive weather application for checking current conditions and forecasts._

## Overview

Welcome to the Weather App! This application provides real-time weather information for cities around the world. Stay informed about current conditions, forecasts, and weather alerts.

## Features

- **Current Weather**: Get up-to-date temperature, humidity, and wind speed
- **5-Day Forecast**: Plan ahead with extended weather predictions
- **Location Search**: Find weather for any city worldwide
- **Weather Alerts**: Stay safe with severe weather notifications
- **Multiple Units**: Switch between Celsius and Fahrenheit

## Getting Started

### Installation

```bash
# Clone the repository
git clone https://github.com/username/weather-app.git

# Navigate to the project directory
cd weather-app

# Install dependencies
npm install

# Start the application
npm start
```

### Usage

1. Enter a city name in the search bar
2. Press Enter or click the Search button
3. View current weather conditions
4. Scroll down for the 5-day forecast

## API Integration

This app uses the OpenWeatherMap API to fetch weather data:

```javascript
const API_KEY = 'your_api_key_here';
const API_URL = 'https://api.openweathermap.org/data/2.5/weather';

async function getWeather(city) {
  const response = await fetch(`${API_URL}?q=${city}&appid=${API_KEY}`);
  const data = await response.json();
  return data;
}
```

## Screenshots

![Weather App Main Screen](https://via.placeholder.com/800x400/4A90E2/ffffff?text=Weather+App+Main+Screen)

## Development Roadmap

- [x] Basic weather display
- [x] City search functionality
- [x] 5-day forecast
- [ ] Hourly forecast
- [ ] Weather maps
- [ ] Mobile app version
- [ ] Dark mode support

## Technology Stack

| Technology | Purpose |
|------------|---------|
| HTML5 | Structure |
| CSS3 | Styling |
| JavaScript | Functionality |
| OpenWeatherMap API | Weather Data |
| LocalStorage | User Preferences |

## Contributing

We welcome contributions! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## Weather Icons

The app uses the following weather condition icons:

- ☀️ Sunny
- ⛅ Partly Cloudy
- ☁️ Cloudy
- 🌧️ Rainy
- ⛈️ Thunderstorm
- ❄️ Snowy
- 🌫️ Foggy

## Support

For questions or issues, please:

- Check our [FAQ](https://github.com/username/weather-app/wiki/FAQ)
- Open an [issue](https://github.com/username/weather-app/issues)
- Contact us at support@weatherapp.com

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

**Made with ❤️ by the Weather App Team**
