# python-api-challenge

### Important!
Please provide your own [Open Weather Map](https://openweathermap.org/api) and [Google Maps](https://developers.google.com/maps/) API keys when running these codes.  You will need to save the Open Weather Map key in a 'config.py' file in the WeatherPy folder, and save the Google Maps API key in a 'config.py' file in the VacationPy folder.

### WeatherPy
A jupyter notebook that gets a random set of latitudes and longitudes and finds the corresponding cities using [citipy](https://pypi.org/project/citipy/).  Uses the random cities to find current weather conditions (with temperature min and max) and plots various weather attributes across latitudes.
Please note that the weather data for this project was collected on 7 February 2021; if you run this notebook during a different time of year, the results may not match up with the discussion/conclusions provided with each plot.

### VacationPy
A jupyter notebook that takes the location and weather data from WeatherPy and plots them on a Google Maps figure.  The list of cities is filtered to find locations with 
- A maximum temperature over 70F but under 80F
- Wind speed less than 10 mph
- No clouds

The Google Maps API is then used to search for the nearest hotel to each lat/long location, and plots these hotels on a map.  Click the map pins to see the name, city, and country of the hotel.