# Code-for-a-Simple-Weather
React.js Code for a Simple Weather App
import React, { useState } from 'react';

function WeatherApp() {
    const [city, setCity] = useState('');
    const [weather, setWeather] = useState('');

    const getWeather = () => {
        // Call weather API and update state
    };

    return (
        <div>
            <input
                type="text"
                value={city}
                onChange={(e) => setCity(e.target.value)}
            />
            <button onClick={getWeather}>Get Weather</button>
            <div>{weather}</div>
        </div>
    );
}

export default WeatherApp;
