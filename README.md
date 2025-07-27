# 🌦️ Power BI Weather, AQI & Forecast Dashboard

This is my first Power BI project — a dynamic dashboard that integrates **live weather data**, **air quality metrics**, and a **7-day forecast** for any selected city using the [WeatherAPI](https://www.weatherapi.com/). The goal was to explore how APIs can be used with Power BI while practicing data transformation, modeling, and visualization.

---

## 📸 Preview

![Dashboard Preview](./FinalDashBoard.png)

---

## 📊 Features

- **Live Weather Data**  
  Displays current temperature, humidity, wind speed, and condition icons for any selected city.

- **Air Quality Index (AQI) Visualization**  
  Shows pollutant levels (PM2.5, NO₂, CO, etc.) with custom DAX-driven color coding and health suggestions.

- **7-Day Forecast**  
  Presents a detailed weekly weather forecast with high/low temperature trend lines and summaries.

- **Interactive Filtering & Comparison**  
  Includes slicers and maps to compare weather and AQI across multiple cities dynamically.

---

## 🧰 Tools & Techniques Used

- **API Integration**  
  - Connected Power BI to the WeatherAPI using Power Query  
  - Parsed and transformed nested JSON responses

- **Power Query**  
  - Cleaned and shaped external data for reporting  
  - Flattened JSON structure and filtered unnecessary fields

- **DAX (Data Analysis Expressions)**  
  - Created reusable measures to color-code AQI status  
  - Added dynamic health suggestions based on pollutant levels

- **Data Visualization**  
  - Designed interactive visuals including cards, gauges, line charts, and maps  
  - Built a user-friendly layout with dynamic city selection

---

## 📦 Data Source

- [WeatherAPI.com](https://www.weatherapi.com/) – for both weather and air quality data

