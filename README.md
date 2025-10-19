# 🌦️ Weather App

A simple and interactive web application that lets users check the current weather conditions for any city in the world using the **OpenWeatherMap API**.

---

## 🚀 Features

* 🌍 Search for any city and get real-time weather updates.
* 🌡️ Displays temperature in Celsius.
* 💧 Shows humidity and wind speed.
* ☁️ Dynamic weather icons that change based on conditions (Rain, Snow, Clouds, etc.).
* ❌ Handles invalid city names with an error message.

---

## 🧰 Technologies Used

* **HTML5** – For the app structure.
* **CSS3** – For styling.
* **JavaScript (ES6)** – For API integration and dynamic updates.
* **OpenWeatherMap API** – For fetching real-time weather data.

---

## 📁 Project Structure

```
📦 Weather App
├── index.html         # Main HTML file
├── script.js          # JavaScript logic and API calls
├── style.css          # Styling
└── images/            # Folder with weather icons
     ├── search.png
     ├── rain.png
     ├── snow.png
     ├── clouds.png
     ├── clear.png
     ├── mist.png
     ├── drizzle.png
     ├── humidity.png
     └── wind.png
```

---

## ⚙️ Setup Instructions

1. **Clone or download** this repository.
2. Open `index.html` in your browser.
3. In `script.js`, replace the existing API key with your own from [OpenWeatherMap](https://openweathermap.org/api):

   ```js
   const apiKey = "YOUR_API_KEY_HERE";
   ```
4. Type a city name in the search box and click the search button.
5. Enjoy real-time weather updates! 🌤️

---

## 🧠 How It Works

1. User enters a city name.
2. JavaScript fetches data from OpenWeatherMap’s API using `fetch()`.
3. The response is converted to JSON using `response.json()`.
4. Weather details (temperature, humidity, wind) are updated dynamically.
5. If the city name is invalid, an error message appears.

---

## 💡 Example API Call

```
https://api.openweathermap.org/data/2.5/weather?q=London&units=metric&appid=YOUR_API_KEY
```

---

## 🐛 Error Handling

If a city is not found (404 response), the app:

* Displays an error message (`Invalid city name`).
* Hides the weather details section.

---

## ✨ Future Improvements

* Add forecast for multiple days.
* Include location-based (GPS) weather detection.
* Improve UI with animations and gradients.