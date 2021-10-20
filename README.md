# Road_trip-ML-Intenship-Project-

PROJECT : Road trip analysis in Newyork city. 

![road-trip](https://user-images.githubusercontent.com/89789110/138128876-bf7c69c4-8109-4e63-acf3-2e80e6893ebd.jpg)


The project we start with taxi data, use this data to make predictions for travel times between locations, and then run the genetic algorithm to optimize the total travel time. We can also read the chart backwards: in order to optimize the travel time, we need to know how long it takes to get from one point to another for each pair of points, and to get that information, we use predictive modeling based on the taxi data.

Since we are given each location’s coordinates, let’s calculate the Manhattan distances between each pair of points and count the longitude and latitude differences to get a sense of direction (East to West, North to South). We can clean up timestamps a little and keep the original features which might look useless to us at first glance.

PROJECT GOAL : The goal of my project is to optimize travel routes for a delivery vehicle by using machine learning model predictions. This is a two-component problem: first, I                train a machine learning model on the data to predict how long it will take a delivery vehicle to go from point one point to another, and I feed these                            predictions into a genetic algorithm which decides which is the most time efficient visit order for a given set of points.

Here is an illustration of my project : dataset  -> machine learning (with xgboost algorithum)  -> optimization with genetic algorithm

![taxi](https://user-images.githubusercontent.com/89789110/138128131-20e8d176-06a0-493f-954a-ff32c4a2dff6.png)

DATA SET :  New York City taxi data set was taken this link  https://www.kaggle.com/c/nyc-taxi-trip-duration/data

MODELS :  After doing a quick baselining with a basic linear regression on the main dataset I realized that a far more complex model was needed. To this end, I selected an                 XGBoost model to accommodate for my complex numeric and categorical features and then i applied generic algorithum for optimization.

ALGORITHUM USED : A genetic algorithm (GA) is a heuristic search algorithm used to solve search and optimization problems. This algorithm is a subset of evolutionary algorithms,                   which are used in computation. Genetic algorithms employ the concept of genetics and natural selection to provide solutions to problems

OPTIMIZATION  : For any given set of locations, these location are fed to the machine learning model, which predicts how long it will take to travel between each two given                       points.Then the algorithm "evolves" to find the visit order which minimizes time spent in transit.

CONCLUSION : The XGBoost model had an error of 4.8 minutes in estimating a single trip's duration for a motor vehicle. While this may seem acceptable for one trip, the error may              get bigger the more locations are visited. The genetic algorithm itself is fairly straightforward, but it must be noted that every genetic algorithm gives an                    optimal approximation, but not the single best solution there is.

OUTPUT SCREENSHOTS : 

output1: Base map using folium 

output2 We had taken 11 waypoints on the map. We would like  to visit all these locations on the same day, and we want to know the best route.
            ![trip  output](https://user-images.githubusercontent.com/89789110/138130924-b75f521d-0e2e-48b2-822a-5879b20411e2.png)


                       





