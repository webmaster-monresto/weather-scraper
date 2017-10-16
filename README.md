# Weather Data Scraper :cloud: :sun_with_face: :cloud:

### Introduction
Bundle of functions used to scrape daily weather data in monthly blocks from [wunderground.com](wunderground.com) (see table at bottom of [this page](https://www.wunderground.com/history/airport/EGLL/2017/10/16/MonthlyHistory.html) for an example of what we'll be scraping).


### Usage
Import by running `from src.scrape_weather import *`

To get weather data for a particular year and month run
```python
get_weather(year=2017, month=1)
```
or simply
```python
get_weather(2017, 1)
```

To get weather data for multiple months in one year
```python
get_weather_multiple_months(years=2017, months=[1, 2, 3])
```

If multiple years are supplied, the code will fetch the full years' data (regardless of which months are supplied)
```python
get_weather_multiple_months(years=range(2000, 2018))
```
