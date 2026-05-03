# 🌤️ Weather App

A React weather forecasting app using the **Open-Meteo API** — completely free, no API key required.

## Features
- Search any city worldwide
- Current weather: temperature, humidity, wind, feels like
- 7-day forecast with daily high/low and rain probability
- Error handling for invalid city names or network failures
- Loading state with spinner
- Fully responsive layout

## Tech Stack
- React 18 + Vite
- CSS Modules (separate file per component)
- Open-Meteo API (free, no API key)
- Custom `useWeather` hook

## Project Structure

```
src/
├── components/
│   ├── SearchBar.jsx        # Search input + button
│   ├── CurrentWeather.jsx   # Main weather card
│   ├── Forecast.jsx         # 7-day forecast section
│   ├── ForecastCard.jsx     # Single day tile
│   ├── StatCard.jsx         # Humidity / Wind / Feels Like
│   ├── ErrorMessage.jsx     # Error banner
│   └── Loader.jsx           # Loading spinner
├── hooks/
│   └── useWeather.js        # All fetching logic (custom hook)
├── utils/
│   ├── api.js               # Geocoding + forecast API calls
│   └── weatherCodes.js      # WMO code → description + emoji
├── styles/
│   ├── App.module.css
│   ├── SearchBar.module.css
│   ├── CurrentWeather.module.css
│   ├── StatCard.module.css
│   ├── Forecast.module.css
│   ├── ForecastCard.module.css
│   ├── ErrorMessage.module.css
│   └── Loader.module.css
├── App.jsx                  # Root component
├── main.jsx                 # Entry point
└── index.css                # Global reset + font import
```

## Getting Started

```bash
npm install
npm run dev
```

Open http://localhost:5173
