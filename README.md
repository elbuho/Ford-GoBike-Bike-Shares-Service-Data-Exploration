# Ford GoBike Bike Shares Service Data Exploration

## Dataset

The data was supplied by Udacity and has a dimension of 183,412 rows by 16 columns that includes information about individual rides in a bike-sharing-system in San Francisco Bay area in  California. The  16 features (variables) are  related with locations of the sation (start and end points), time duration of the trip, user type and gender. 100% of the data correspond to the month of February 2017 in the start_time variable, so my analysis is not monthly, it is focused on the days of the week and the hours of the day in which the service is used. It is also focused on start station and start_time.
More exhaustively, the relationship of variables is as follows:

* Original variables in the dataset:  

    + duration_sec: Trip durationDuration in seconds
    + start_time: Start time and date as string
    + end_time: End Time and Date as string
    + start_station_id: Start station id
    + start_station_name: Name of the start station
    + start_station_latitude: Latitude of the start station
    + start_station_longitude: Longitude of the start station
    + end_station_id: End Station id
    + end_station_name: End station name
    + end_station_latitude: Latitude of the end station
    + end_station_longitude: Longitude of the end station
    + bike_id: bike ID
    + user_type: User Type it can be Subscriber or Customer
    + member_birth_year: member year of birth
    + member_gender: member gender
    + bike_share_for_all_trip: Boolean 
    


* Variables created to enrich the analysis:  
    + start_hour: start hour in format from 0 to 24
    + start_day: days of the week
    + start_month: start month
    + end_hour: end hour in format from 0 to 24
    + end_month: end month 
    + duration: duration in minutes
    

## Summary of Findings

* Univariate exploration:
We found that Market St at 10th ST has more rides in total trips, follow by San Francisco Caltrain Station 2 and Berry St at 4th St. We have only considered (start points). Thursday has more total trips, followed by Tuesday and Wednesday. There is a significant decrease in the number of trips on weekends.
17: 00 hour in the afternoon and 8:00 in the morning present the highest number of total trips.
Male has 75% of the total ride and the subscribers are the 91% of the total user type if we consider all the trips. The average year of birth of all the riders is 1984 and they spend on average 11.74 minutes by trip. The average of the duration is greater on weekends for all riders.

* Bivariate Exploration:
The corralation between  age and duration of trips is so weak close to cero. Average trip duration is longer on weekends than on work days. We see that customers spend more time on average than subscribers and that the average duration of trips by genre does not change much. The hourly distribution by subscribers for the trips made presents two clear peaks (bimodal) in the morning and another in the afternoon.

* Multivariate exploration:
Females have longer travel durations than males every day of the week. Customers spend more time on average every day of the week than subscribers. Males have more than twice as many trips as females every day of the week. San Francisco Caltrain Station 2 is the busiest station from Monday to Thursday, but on Fridays Market St at 10th St stations is busiest and on weekends too. Subscribers concentrate most of their trips between 7 and 9 in the morning and between 16 and 18 in the afternoon during working hours.


## Key Insights for Presentation

San Francisco Caltrain Station 2 is and Market St at 10th St. are the busiest stations. We have to take into account that the types of users have an important role in the number of trips made and even in their duration. Customers generally have longer trips than subscribers on all days of the week and during daylight hours. Subscribers make much more use of the service during business hours.


