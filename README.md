This project is a simple weather application that allows users to get weather information based on their current location or by searching for a city.

Features-
  1. Current Location Weather: Users can grant location access to get weather information for their current location.
  2. Search Weather: Users can search for weather information by entering a city name.
  3. Weather Details: Displays city name, country flag, weather description, temperature, wind speed, humidity, and cloudiness.
  4. Loading Indicator: Shows a loading screen while fetching weather data.
     
Technologies Used- HTML, CSS, JavaScript, OpenWeather API, Setup and Usage.

Prerequisites- Web browser with JavaScript enabled.
              Internet connection to fetch weather data from the OpenWeather API.
  
Installation-
  Clone the repository:
    bash
      git clone https://github.com/your-repository/weather-app.git
      
  Navigate to the project directory:
    bash
      cd weather-app
    
Running the Application-
  Open index.html in your web browser.
  
Functionality-
  Switch Tabs
    1. Your Weather Tab: Displays weather information for the user's current location.
    2. Search Weather Tab: Allows users to search for weather information by entering a city name.
  Grant Location Access
    1. When the user clicks on the "Grant Access" button, the browser will request permission to access the user's location.
        If permission is granted, the app will fetch and display weather information for the user's current location.
        Search Weather
    2. Users can search for weather information by entering a city name in the search box and clicking the search button.
        The app will fetch and display weather information for the entered city.
      
Code Explanation-

    HTML Structure
      The HTML file defines the structure of the application, including the tab navigation, location access prompt, search form, loading screen, and weather information display.
    CSS Styling
      The CSS file (style.css) styles the application, including the layout, colors, and responsiveness.
    JavaScript Functionality
      The JavaScript file (script.js) handles the application's functionality, including tab switching, location access, fetching weather data, and updating the UI.
      Key JavaScript Functions
        1. switchTab: Switches between the "Your Weather" and "Search Weather" tabs.
        2. getfromSessionStorage: Checks if user coordinates are stored in session storage and fetches weather information if available.
        3. fetchUserWeatherInfo: Fetches weather information based on the user's coordinates.
        4. renderWeatherInfo: Updates the UI with fetched weather data.
        5. getLocation: Requests the user's current location.
        6. showPosition: Stores the user's coordinates in session storage and fetches weather information.
        7. fetchSearchWeatherInfo: Fetches weather information based on the searched city name.
    API Integration
        The app uses the OpenWeather API to fetch weather data.
        An API key is required to use the OpenWeather API. Replace the placeholder API_KEY in the JavaScript file with your actual API key.
        
Notes-
  1. Ensure that the browser has location services enabled for accurate weather information.
  2. Handle errors gracefully, such as when location access is denied or the API call fails.
