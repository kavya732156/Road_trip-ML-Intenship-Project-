# Road_trip-ML-Intenship-Project-

PROJECT : Road trip analysis in Newyork city. 

The project we start with taxi data, use this data to make predictions for travel times between locations, and then run the genetic algorithm to optimize the total travel time. We can also read the chart backwards: in order to optimize the travel time, we need to know how long it takes to get from one point to another for each pair of points, and to get that information, we use predictive modeling based on the taxi data.

Since we are given each location’s coordinates, let’s calculate the Manhattan distances between each pair of points and count the longitude and latitude differences to get a sense of direction (East to West, North to South). We can clean up timestamps a little and keep the original features which might look useless to us at first glance.

PROJECT GOAL : The goal of my project is to optimize travel routes for a delivery vehicle by using machine learning model predictions. This is a two-component problem: first, I                  train a machine learning model on the data to predict how long it will take a delivery vehicle to go from point one point to another, and I feed these predictions                  into a genetic algorithm which decides which is the most time efficient visit order for a given set of points.




