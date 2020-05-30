# Analysis of NYC Vehicle Collisions
Contributors: Caroline Barker and Andrew Liang \
Created: 4.20.20

## Objective
We focused our efforts on addressing which areas should be targeted for redesign efforts. We wanted to expose problematic areas that had high or abnormal collisions, that civil engineers or road engineers could investigate for improvement.


## Dataset
[NYC OpenData Motor Vehicle Collisions - Crashes](https://data.cityofnewyork.us/Public-Safety/Motor-Vehicle-Collisions-Crashes/h9gi-nx95) \
Each row object represents a crash event and includes details on each event and has been updated daily since 5.7.14. It includes 29 columns 
(attributes) for each crash, of which we focus on the following: 

Column Name | Description | Type
------------ | -------------| -------------
CRASH DATE | Occurrence date of collision | Date & Time
CRASH TIME | Occurence time of collision | Text
BOROUGH | Borough where collision occured| Text
ZIPCODE | Postal code of incident occurence| Text
LONGITUDE | Longitude coordinate for Global Coordinate System | Number
LATITUDE | Latitude coordinate for Global Coordinate System | Number
NUMBER OF PEDESTRIANS INJURED | Number of pedestrians injured | Number
NUMBER OF PEDESTRIANS KILLED | Number of pedestrians killed | Number
NUMBER OF CYCLISTS INJURED | Number of cyclists injured | Number
NUMBER OF CYCLISTS KILLED | Number of cyclists killed | Number
NUMBER OF MOTORISTS INJURED | Number of motorists injured | Number
NUMBER OF MOTORISTS KILLED | Number of motorists killed | Number


## Question 1: Which places are the most collisions prone?
We addressed this question with a geographic map that represents data across all years in the dataset. Coordinates are rounded to 8 decimal places and their radius corresponds to the number of collisions. They are color coded by standard deviations away from the mean, so that we can identify collision hotspots more easily. The red points or circles are places that are three standard deviations away from the mean, and are the hotspots we identified. On the opposite end of the spectrum, blue points are points below the 50th percentile.

![Preliminary Map](https://github.com/CarolineNB/Large-Scale-Visual-Analytics/blob/master/NY%20Vehicle%20Collisions/demos/Standard%20Deviation.PNG)
