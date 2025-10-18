<div align="center">

# 🌦️ Power BI Weather, AQI & Forecast Dashboard

![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=for-the-badge&logo=powerbi&logoColor=black)
![API](https://img.shields.io/badge/Weather_API-Integration-00D4FF?style=for-the-badge)
![DAX](https://img.shields.io/badge/DAX-Measures-FF6B6B?style=for-the-badge)
![Data Visualization](https://img.shields.io/badge/Data_Viz-Interactive-4CAF50?style=for-the-badge)

**An interactive Power BI dashboard integrating live weather data, air quality metrics, and 7-day forecasts for real-time environmental insights**

[![View Project](https://img.shields.io/badge/📊_View_Project-Power_BI-F2C811?style=for-the-badge)](#)

[Features](#-features) • [Tools & Techniques](#-tools--techniques-used) • [Installation](#-installation) • [Data Model](#-data-model) • [Insights](#-key-insights)

---

<img src="https://github.com/PasinduSuraweera/Weather-Dashboard-w-Power-BI/blob/main/FinalDashBoard.png?raw=true" alt="Weather Dashboard Preview" width="900px" />

</div>

## 📋 Overview

The **Power BI Weather, AQI & Forecast Dashboard** is a comprehensive data visualization project that transforms real-time weather and air quality data into actionable insights. This is my first Power BI project, designed to explore the intersection of **API integration**, **data transformation**, and **interactive visualization**.

Built using data from **WeatherAPI.com**, this dashboard provides a complete environmental picture for any city worldwide, combining current conditions, pollution metrics, and future forecasts in an intuitive, user-friendly interface.

Whether you're a weather enthusiast, environmental analyst, or data professional, this dashboard demonstrates the power of Power BI in creating dynamic, data-driven decision-making tools.

## ✨ Features

### 🌡️ **Live Weather Data**
Real-time weather information at your fingertips:
- **Current Temperature** - Displayed in Celsius/Fahrenheit with dynamic icons
- **Humidity Levels** - Moisture content percentage
- **Wind Speed & Direction** - Complete wind metrics
- **Weather Conditions** - Visual representation with condition icons
- **"Feels Like" Temperature** - Apparent temperature calculations
- **UV Index** - Sun exposure levels
- **Visibility** - Atmospheric clarity measurements

### 🏭 **Air Quality Index (AQI) Visualization**
Comprehensive pollution monitoring and health insights:
- **PM2.5 Levels** - Fine particulate matter concentration
- **PM10 Levels** - Coarse particulate matter
- **NO₂ (Nitrogen Dioxide)** - Traffic-related pollutant
- **CO (Carbon Monoxide)** - Combustion byproduct
- **O₃ (Ozone)** - Ground-level ozone levels
- **SO₂ (Sulfur Dioxide)** - Industrial pollutant
- **Custom Color Coding** - DAX-driven visual indicators
- **Health Recommendations** - Dynamic suggestions based on AQI levels

### 📅 **7-Day Weather Forecast**
Detailed weekly outlook with trend analysis:
- **Daily High/Low Temperatures** - Temperature range predictions
- **Trend Line Visualizations** - Temperature pattern analysis
- **Weather Condition Summaries** - Daily forecast descriptions
- **Precipitation Probability** - Rain/snow chances
- **Sunrise/Sunset Times** - Daylight hours tracking

### 🗺️ **Interactive City Selection**
Dynamic filtering and comparison capabilities:
- **City Slicer** - Quick location switching
- **Geographic Maps** - Visual location representation
- **Multi-City Comparison** - Side-by-side analysis
- **Saved Favorites** - Quick access to frequently viewed cities
- **Search Functionality** - Find any city worldwide

### 📊 **Advanced Visualizations**
Professional-grade visual components:
- **KPI Cards** - Key metrics at a glance
- **Gauge Charts** - Visual indicators for ranges
- **Line Charts** - Trend analysis over time
- **Maps** - Geographic data representation
- **Custom Tooltips** - Detailed hover information
- **Responsive Layout** - Adapts to screen sizes

## 🛠️ Tools & Techniques Used

<div align="center">

### **Core Technologies**

| Technology | Purpose | Complexity |
|------------|---------|------------|
| ![Power BI](https://img.shields.io/badge/Power_BI-F2C811?style=flat&logo=powerbi&logoColor=black) | Data visualization and dashboard creation | Advanced |
| ![Power Query](https://img.shields.io/badge/Power_Query-00A4EF?style=flat) | Data transformation and ETL processes | Intermediate |
| ![DAX](https://img.shields.io/badge/DAX-FF6B6B?style=flat) | Calculated measures and custom logic | Advanced |
| ![WeatherAPI](https://img.shields.io/badge/Weather_API-00D4FF?style=flat) | Real-time weather and AQI data source | Integration |

</div>

### 🔌 **API Integration**
- **REST API Connection** - Direct integration with WeatherAPI.com
- **Power Query M Language** - Custom API queries and parameters
- **JSON Parsing** - Handling nested JSON response structures
- **Authentication Management** - Secure API key storage
- **Error Handling** - Graceful failure management
- **Rate Limiting** - Efficient API call optimization

### 🔄 **Power Query Transformation**
- **Data Cleansing** - Removing nulls and invalid entries
- **JSON Flattening** - Converting nested structures to tabular format
- **Data Type Conversion** - Ensuring proper field types
- **Column Filtering** - Removing unnecessary fields
- **Data Refresh Configuration** - Scheduled update setup
- **Query Folding** - Performance optimization

### 📐 **DAX (Data Analysis Expressions)**
- **Custom Measures** - Reusable calculation logic
- **Conditional Formatting** - Dynamic color coding based on values
- **Health Status Calculations** - AQI-based recommendations
- **Time Intelligence** - Date-based calculations
- **Aggregation Functions** - Statistical summaries
- **SWITCH Statements** - Complex conditional logic

### 🎨 **Data Visualization Techniques**
- **Color Psychology** - Using colors to convey information
- **Visual Hierarchy** - Organizing information by importance
- **White Space Management** - Clean, uncluttered design
- **Interactive Elements** - Slicers, filters, and drill-through
- **Custom Themes** - Brand-consistent color schemes
- **Accessibility** - High contrast and readable fonts

## 🏗️ System Architecture

```
┌─────────────────────────────────────────────────────────────┐
│                    POWER BI DASHBOARD                       │
│                                                             │
│  ┌──────────────┐  ┌──────────────┐  ┌──────────────────┐ │
│  │   Current    │  │   Air Quality│  │   7-Day          │ │
│  │   Weather    │  │   Index (AQI)│  │   Forecast       │ │
│  │   Visuals    │  │   Visuals    │  │   Visuals        │ │
│  └──────────────┘  └──────────────┘  └──────────────────┘ │
│         │                 │                    │            │
│         └─────────────────┴────────────────────┘            │
│                           │                                 │
│                  ┌────────▼────────┐                       │
│                  │   DAX Measures  │                       │
│                  │   - AQI Status  │                       │
│                  │   - Health Tips │                       │
│                  │   - Calculations│                       │
│                  └────────┬────────┘                       │
└───────────────────────────┼─────────────────────────────────┘
                            │
                   ┌────────▼────────┐
                   │  Data Model     │
                   │  - Weather Table│
                   │  - Forecast     │
                   │  - AQI Table    │
                   │  - Location     │
                   └────────┬────────┘
                            │
┌───────────────────────────▼─────────────────────────────────┐
│                    POWER QUERY EDITOR                       │
│                                                             │
│  ┌─────────────────────────────────────────────────────┐  │
│  │              Data Transformation                     │  │
│  │  - JSON Parsing                                     │  │
│  │  - Data Cleansing                                   │  │
│  │  - Field Extraction                                 │  │
│  │  - Type Conversion                                  │  │
│  └─────────────────────────────────────────────────────┘  │
└────────────────────────────┬────────────────────────────────┘
                             │
                    ┌────────▼────────┐
                    │  Weather API    │
                    │  weatherapi.com │
                    │                 │
                    │  Endpoints:     │
                    │  - /current.json│
                    │  - /forecast    │
                    │  - /air_quality │
                    └─────────────────┘
```

## 🎯 Data Model

### **Tables & Relationships**

```
Weather Data (Fact Table)
├── Temperature
├── Humidity
├── Wind Speed
├── Condition
├── Timestamp
└── Location_ID (FK)

Forecast Data (Fact Table)
├── Date
├── High Temperature
├── Low Temperature
├── Condition
├── Precipitation %
└── Location_ID (FK)

Air Quality Data (Fact Table)
├── PM2.5
├── PM10
├── NO₂
├── CO
├── O₃
├── SO₂
├── AQI Index
├── Timestamp
└── Location_ID (FK)

Location (Dimension Table)
├── Location_ID (PK)
├── City Name
├── Country
├── Latitude
└── Longitude
```

## 📥 Installation & Setup

### Prerequisites
- **Power BI Desktop** (Latest version recommended)
- **WeatherAPI Account** ([Sign up here](https://www.weatherapi.com/signup.aspx))
- **Internet Connection** - For API data refresh

### Step-by-Step Setup

1. **Get Your API Key**
```
1. Visit https://www.weatherapi.com/signup.aspx
2. Create a free account
3. Navigate to "My Account" > "API Key"
4. Copy your API key
```

2. **Clone the Repository**
```bash
git clone https://github.com/PasinduSuraweera/Weather-Dashboard-w-Power-BI.git
cd Weather-Dashboard-w-Power-BI
```

3. **Open Power BI File**
```
- Open Power BI Desktop
- File > Open > Browse
- Select the .pbix file from the repository
```

4. **Configure API Key**
```
- Transform Data > Power Query Editor
- Select "WeatherAPI" query
- Update the API_KEY parameter with your key
- Close & Apply
```

5. **Refresh Data**
```
- Home > Refresh
- Wait for data to load (usually 10-30 seconds)
- Dashboard will populate with live data
```

6. **Customize Settings**
```
- Select your preferred city in the slicer
- Adjust date range for forecasts
- Configure refresh schedule (optional)
```

## 🚀 Usage Guide

### Viewing Current Weather
1. Select a city from the dropdown slicer
2. View real-time temperature, humidity, and wind data
3. Check weather condition icon and description
4. Note the "feels like" temperature for planning

### Analyzing Air Quality
1. Navigate to the AQI section
2. Review pollutant levels with color-coded indicators:
   - 🟢 **Green** - Good (0-50)
   - 🟡 **Yellow** - Moderate (51-100)
   - 🟠 **Orange** - Unhealthy for Sensitive Groups (101-150)
   - 🔴 **Red** - Unhealthy (151-200)
   - 🟣 **Purple** - Very Unhealthy (201-300)
   - 🟤 **Maroon** - Hazardous (301+)
3. Read health recommendations based on current AQI

### Exploring 7-Day Forecast
1. View daily high/low temperature predictions
2. Analyze temperature trends with line charts
3. Check precipitation probability for outdoor planning
4. Note sunrise/sunset times for each day

### Comparing Multiple Cities
1. Use the map visual to select multiple locations
2. Compare temperature, AQI, and forecast data side-by-side
3. Identify patterns across different regions

## 📊 Key DAX Measures

### AQI Status Color Coding
```dax
AQI_Status = 
SWITCH(
    TRUE(),
    [AQI_Value] <= 50, "Good",
    [AQI_Value] <= 100, "Moderate",
    [AQI_Value] <= 150, "Unhealthy for Sensitive",
    [AQI_Value] <= 200, "Unhealthy",
    [AQI_Value] <= 300, "Very Unhealthy",
    "Hazardous"
)
```

### Health Recommendations
```dax
Health_Suggestion = 
SWITCH(
    [AQI_Status],
    "Good", "Air quality is excellent. Enjoy outdoor activities!",
    "Moderate", "Air quality is acceptable for most people.",
    "Unhealthy for Sensitive", "Sensitive groups should limit outdoor activities.",
    "Unhealthy", "Everyone should reduce prolonged outdoor exertion.",
    "Very Unhealthy", "Health alert: Everyone may experience health effects.",
    "Hazardous", "Emergency conditions. Avoid outdoor activities."
)
```

### Temperature Trend
```dax
Temp_Trend = 
VAR CurrentTemp = [Current_Temperature]
VAR PreviousTemp = CALCULATE([Current_Temperature], DATEADD('Date'[Date], -1, DAY))
RETURN
    IF(CurrentTemp > PreviousTemp, "▲ Rising", "▼ Falling")
```

## 🔮 Key Insights & Learnings

### What I Learned
- ✅ **API Integration in Power BI** - Connecting external data sources
- ✅ **JSON Data Handling** - Parsing complex nested structures
- ✅ **DAX Mastery** - Creating dynamic, reusable measures
- ✅ **Visual Design** - Building intuitive, user-friendly dashboards
- ✅ **Data Modeling** - Establishing relationships between tables
- ✅ **Performance Optimization** - Query folding and efficient refreshes

### Challenges Overcome
- 🎯 Flattening nested JSON responses from the API
- 🎯 Creating dynamic color coding based on multiple conditions
- 🎯 Managing API rate limits and refresh schedules
- 🎯 Designing responsive layouts for different screen sizes
- 🎯 Implementing error handling for missing data

### Business Applications
- 📈 **Agriculture** - Crop planning and irrigation scheduling
- 🏗️ **Construction** - Weather-dependent project management
- 🚚 **Logistics** - Route planning and delivery optimization
- ⚡ **Energy** - Renewable energy production forecasting
- 🏥 **Healthcare** - Air quality health alerts and monitoring

## 📦 Data Source

### WeatherAPI.com
**Primary data provider for all weather and air quality information**

- 🌐 Website: [https://www.weatherapi.com](https://www.weatherapi.com/)
- 📚 Documentation: [API Docs](https://www.weatherapi.com/docs/)
- 🆓 Free Tier: 1 million calls/month
- 🌍 Coverage: 200+ countries worldwide
- 📡 Update Frequency: Real-time (every 15 minutes)

**Available Endpoints:**
- `/current.json` - Real-time weather data
- `/forecast.json` - Multi-day forecasts
- `/history.json` - Historical weather data
- `/search.json` - Location search
- `/astronomy.json` - Sunrise/sunset data

## 🎨 Design Principles

### Visual Hierarchy
- **Primary Information** - Large, bold current weather
- **Secondary Information** - AQI and forecast data
- **Tertiary Information** - Additional details in tooltips

### Color Scheme
- **Blue Tones** - Temperature and weather conditions
- **Green/Red Gradient** - Air quality indicators
- **Neutral Background** - White/light gray for clarity
- **Accent Colors** - Yellow/orange for highlights

### User Experience
- **Minimal Clicks** - Key information visible immediately
- **Intuitive Navigation** - Logical flow between sections
- **Responsive Design** - Works on various screen sizes
- **Fast Loading** - Optimized queries for quick refresh

## 🔒 Best Practices

### Data Refresh
- ⏰ Schedule automatic refreshes during off-peak hours
- 🔄 Set reasonable refresh intervals (every 15-60 minutes)
- 📊 Monitor refresh history for failures
- 💾 Use incremental refresh for historical data

### Performance
- ⚡ Use query folding where possible
- 📦 Remove unnecessary columns in Power Query
- 🎯 Optimize DAX measures for efficiency
- 💾 Consider aggregations for large datasets

### Security
- 🔐 Store API keys securely (don't share .pbix with keys)
- 🛡️ Use parameters for sensitive information
- 🔒 Implement row-level security if sharing dashboard
- ✅ Validate data sources before publishing

## 🤝 Contributing

Contributions and suggestions are welcome! Help improve this dashboard.

### How to Contribute:

1. **Fork the Project**
2. **Create your Feature Branch**
   ```bash
   git checkout -b feature/AmazingFeature
   ```
3. **Commit your Changes**
   ```bash
   git commit -m 'Add some AmazingFeature'
   ```
4. **Push to the Branch**
   ```bash
   git push origin feature/AmazingFeature
   ```
5. **Open a Pull Request**

### Contribution Ideas:
- 🌡️ Additional weather metrics
- 📊 New visualization types
- 🎨 Custom themes and color schemes
- 🌍 Multi-language support
- 📱 Mobile-optimized layouts
- 🔔 Alert thresholds and notifications

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👤 Author

**Pasindu Suraweera**

- 🐙 GitHub: [@PasinduSuraweera](https://github.com/PasinduSuraweera)
- 💼 LinkedIn: [Connect with me](#)
- 📧 Email: [Contact me](#)

## 🙏 Acknowledgments

- 🌦️ [WeatherAPI.com](https://www.weatherapi.com/) - Comprehensive weather data API
- 📊 [Microsoft Power BI](https://powerbi.microsoft.com/) - Powerful data visualization platform
- 🎨 Power BI Community - Inspiration and best practices
- 📚 DAX.guide - DAX formula reference and examples
- 💙 Open data community for environmental monitoring initiatives

## 📞 Support

Need help or have questions?

- 🐛 [Report a Bug](https://github.com/PasinduSuraweera/Weather-Dashboard-w-Power-BI/issues)
- 💡 [Request a Feature](https://github.com/PasinduSuraweera/Weather-Dashboard-w-Power-BI/issues)
- 💬 [Ask a Question](https://github.com/PasinduSuraweera/Weather-Dashboard-w-Power-BI/discussions)

## 🎓 Learning Resources

### Power BI
- [Microsoft Power BI Documentation](https://docs.microsoft.com/en-us/power-bi/)
- [SQLBI - DAX Patterns](https://www.daxpatterns.com/)
- [Power BI Community Forums](https://community.powerbi.com/)

### DAX
- [DAX Guide](https://dax.guide/)
- [DAX Formatter](https://www.daxformatter.com/)
- [SQLBI Video Courses](https://www.sqlbi.com/)

### Data Visualization
- [Storytelling with Data](http://www.storytellingwithdata.com/)
- [Power BI Design Best Practices](https://docs.microsoft.com/en-us/power-bi/create-reports/power-bi-visualization-best-practices)

---

<div align="center">

### ⭐ **If you find this dashboard useful, please give it a star!** ⭐

**Made with 📊 and ❤️ by Pasindu Suraweera**

![Visitors](https://visitor-badge.laobi.icu/badge?page_id=PasinduSuraweera.Weather-Dashboard-w-Power-BI)

*Transforming weather data into actionable insights* 🌦️

</div>
