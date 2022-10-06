# PyBer Ridesharing Analysis

# Overview
## Purpose
The purpose of this project is to create a graphical summary of rideshare fares over the time frame from 01/01/2019 to 04/29/2019. The data covered a sample of rides in cities that which were categorized as Urban, Suburban and Rural with the intent of understanding rate differences by those three categories.
## Approach
The analylsis required the use of two separate data sources for city data (city_data.csv) and ride data(ride_data.csv). The city data contained the name of the city, the driver count for the city and the type of city, either Urban, Suburban or Rural. The ride data contained the city name, the data=e of the ride, the fare paid and the ride_id. The city name was used as the key to match the two data sets, which allowed for the type of city to be associated with each ride and for a summary of the data to be created by the type of city.

Once the data sets were understood and joined, the date field, which was took a datetime format in the original data set, was translated to dates only removing the time element. This allowed the data to be represented in consistent time intervals of whole days. By doing this, the data was consistent and comparable between categories at more relvant intervals. The data was then represented visually using a line graph with each type of city represented by a different color. A title, and label for the x axis were added along with a key so that the user can better understand the information being presented.

# Results
## Total Summary Data
For the total data set, summary statistics are shown in the table below. The table shows that, within this data set, Urban cities have more total rides and drivers as well has higher total fares. Urban cities have more drivers than rides, meaning that some drivers must not be giving any rides. Urban cities also have the highest Average Fare per Ride, followed by Suburban cities and then Rural cities. Rural cities have the highest Average Fare per Driver, followed by Suburban cities and then Urban cities.

![PyBer Data Summary](https://github.com/jessica1258/PyBer_Analysis/blob/main/analysis/PyBer_data_summary.png)

## Select Data from January through April (01/01/2019 to 04/29/2019)
Based on the line graph (shown below), the Urban cities see the highest total fares, followed by Suburban and Rural cities for the selected subset of data. This is a consistent outcome despite fluctuations in the fares observed over time. This result is consistent with the original summary data, which contained a higher ride count for Urban cities.

![PyBer Fare Summary](https://github.com/jessica1258/PyBer_Analysis/blob/main/analysis/PyBer_fare_summary.png)

# Recommendations
In order to address disparities by city types, there are three key recommendations. First, further analysis is required to understand per ride fare differences in the three types of cities. This analysis should be focused on additional ride features such as driving distance to understand if per ride fare differences are a result of underlying differences in the rides or due to the ratio of drivers to rides. Second, the CEO should understand why some drivers in Urban cities are not giving rides and whether this represents a missed opportunity for supplying additional rides to customers. Third, the CEO should understand fluctuations in the daily fares to understand if specific days or times of day result in higher per ride fares or a higher number of rides.
