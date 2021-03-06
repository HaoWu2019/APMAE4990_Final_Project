# APMAE4990_Final_Project

## NYC Taxi ETA

This project aims to build different models to predict travel time between two points in New York City by using the New York yellow cab data in 2016 from Big Query.

The models we built include **Linear Regression Model**, **Regularization Linear Model (Lasso)**, **Decision Tree Model**, and **Random Forest Model**.

## The features we used:

`visib`: Countinuous variable. The mean visibility for the day in miles.

`wdsp`: Continuous variable. The mean wind speed for the day in knots.

`temp`: Continuous variable. The mean temperature for the day in degrees Fahrenheit.

`fog`: Categorical variable. Indicators for the occurrence of fog during the day (1 = yes and 0 = no/not reported).

`rain_drizzle`: Categorical variable. Indicators for the occurrence of rain during the day (1 = yes and 0 = no/not reported).

`snow_ice_pellets`: Categorical variable. Indicators for the occurrence of snow during the day (1 = yes and 0 = no/not reported).

`week_index`: Categorical variable. Indicators for the weekdays and weekends (1 = Monday-Friday and 0 = Saturday-Sunday).

`rain_level`: Categorical variables. Indicators for the rain levels of the day. There are four levels including no rain, light rain, moderate rain, and heavy rain. There are 3 dummy variables in total for the rain_level feature.

`rush_hour_ind`: Categorical variable. Indicators for rush hour and off-peak hour in New York city (1 = 7-10AM, 3-7PM and 0 = the remaining hours).

`distance_in_km`: Continuous variable. Haversine distance measures the shortest path distance between two points on the sphere. 

`avg_travel_time`: Continuous variable. The average **historical** travel time in terms of the same *pickup area* and *drop-off area*, with geohash precision = 6. For example, if someone is traveling from abcdef (geohash code) to abcdeg (geohash code) at 15:00 on May 15th. The `avg_travel_time` will calculate the average travel time for trips that traveled from abcdef to abcdeg before May 15th 15:00. 

`avg_hr_travel_time`: Continuous variable. The average **historical** travel time in terms of the same *pickup area*, *drop-off area*, and *pickup hour*, with geohash perceision = 6. For example, if someone is traveling from abcdef (geohash code) to abcdeg (geohash code) at 15:00 on May 15th. The `avg_hr_travel_time` will calculate the average travel time for trips that happened at 15:00 and traveled from abcdef to abcdeg before May 15th 15:00. 

`avg_trip_dist`: Continuous variable. The average **historical** trip distance in terms of the same *pickup area* and *drop-off area*, with geohash precision = 6. For example, if someone is traveling from abcdef (geohash code) to abcdeg (geohash code) at 15:00 on May 15th. The `avg_trip_dist` will calculate the average trip distance for trips that traveled from abcdef to abcdeg before May 15th 15:00. 

`avg_hr_trip_dist`: Continuous variable. The average **historical** trip distance in terms of the same *pickup area*, *drop-off area*, and *pickup hour*, with geohash perceision = 6. For example, if someone is traveling from abcdef (geohash code) to abcdeg (geohash code) at 15:00 on May 15th. The `avg_hr_trip_dist` will calculate the average trip distance for trips that happened at 15:00 and traveled from abcdef to abcdeg before May 15th 15:00.

`avg_fare_amount`: Continuous variable. The average **historical** fare amount in terms of the same *pickup area* and *drop-off area*, with geohash precision = 6. For example, if someone is traveling from abcdef (geohash code) to abcdeg (geohash code) at 15:00 on May 15th. The `avg_fare_amount` will calculate the average fare amount for trips that traveled from abcdef to abcdeg before May 15th 15:00. 

`avg_hr_fare_amount`: Continuous variable. The average **historical** fare amount in terms of the same *pickup area*, *drop-off* area, and *pickup hour*, with geohash perceision = 6. For example, if someone is traveling from abcdef (geohash code) to abcdeg (geohash code) at 15:00 on May 15th. The `avg_hr_fare_amount` will calculate the average fare amount for trips that happened at 15:00 and traveled from abcdef to abcdeg before May 15th 15:00.


## Contribution

**Xin Xia**: Xin Xia is responsible for hyperparameters tuning and final prediction.

**Haofeng Chen**: Haofeng Chen is responsible for feature engineering and model selection.

**Hao Wu**: Hao Wu is responsible for exploratory data analysis and integrity check.

**Caihui Xiao**: Caihui Xiao is responsible for bigquery SQL and combining weather data.
