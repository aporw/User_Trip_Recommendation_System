# User_Trip_Recommendation_System

![What is this](trip_recomm.jpg)
Solving the problem of Flight Booking company on how to recommend trips to user 

# Identifying features for similar trip:

1. Departure date
2. Arrival date ( for two-way)
3. Departure Aiport
4. Arrival Airport
5. Stay
6. Weekend 
7. Non_stop
8. Layover time

 Similarity measures: Minimum Ecludian distance, Cosine Similarity

 Grouping users and finding trip most similar to their previous trips.

# Multi Output Neural Network

Can we create a mapping between unsuccessful trips to successful trips for users? Successful means trips which are booked or active.

Built a multi-output neural network with optimizing loss for all 4 outputs.

Predicted Lattitude- Longitude for destination, Number of days from 1/1/2015 for departure date and total stay for return date. 

The origin is same as trip which is search is last 1 month by the user. 

Once all above attibutes are known, we can recommned a trip: (origin, destination, departure_date, return_date)


