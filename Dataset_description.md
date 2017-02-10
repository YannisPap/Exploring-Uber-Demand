### Name:
**Uber.csv**

###Description:
The dataset contains information for Uber pickups, weather conditions and public holidays for the NYC for the period 2015-01-01 - 2015-06-30.

### Sources:

* Uber Pickups in New York City, from 01/01/2015 to 30/06/2015. (by [kaggle.com](https://www.kaggle.com/fivethirtyeight/uber-pickups-in-new-york-city))  
* Weather data from [National Centers for Environmental Information](https://www.ncdc.noaa.gov/).  
* LocationID to Borough mapping. (by [FiveThirtyEight](https://github.com/fivethirtyeight/uber-tlc-foil-response/blob/master/uber-trip-data/taxi-zone-lookup.csv))  
* NYC public holidays.   

### Variables:
| Name      | Description                      | Type                                                                                    | Units      |
|-----------|----------------------------------|-----------------------------------------------------------------------------------------|------------|
| pickup_dt | Time period of the observations. | POSIXct                                                                                 |            |
| borough   | NYC's borough                    | factor with 6 levels: "Manhattan", "Brooklyn", Queens", "Bronx", "Staten Island", "EWR" |            |
| pickups   | Number of pickups for the period | numeric                                                                                 |            |
| spd       | Wind speed                       | numeric                                                                                 | miles/hour |
| vsb       | Visibility                       | numeric                                                                                 | miles      |
| temp      | Temperature                      | numeric                                                                                 | fahrenheit |
| dewp      | Dew point                        | numeric                                                                                 | fahrenheit |
| slp       | Sea level pressure               | numeric                                                                                 | millibars  |
| pcp01     | 1-hour liquid precipitation      | numeric                                                                                 | inches     |
| pcp06     | 2-hours liquid precipitation     | numeric                                                                                 | inches     |
| pcp24     | 24-hours liquid precipitation    | numeric                                                                                 | inches     |
| sd        | Snow depth in inches             | numeric                                                                                 | inches     |
| hday      | Holiday                          | factor with 2 levels: "Y", "N"                                                          |            |
