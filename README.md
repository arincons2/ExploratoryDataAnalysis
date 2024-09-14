# ExploratoryDataAnalysis

Exploratory Data Analysis for food order, performed in python. 
It was originally developed in Google colab.
It is necessary to charge the data (foodhub_order.csv).
Probably, the path (path_foodhub) must be changed in order to correctly charge the data. 
You can download the two files (the ipynb and the csv files) and upload them in your personal google drive and run. It is easy.    

Data Description
The data contains the different data related to a food order. The detailed data dictionary is given below.

Data Dictionary
order_id: Unique ID of the order
customer_id: ID of the customer who ordered the food
restaurant_name: Name of the restaurant
cuisine_type: Cuisine ordered by the customer
cost: Cost of the order
day_of_the_week: Indicates whether the order is placed on a weekday or weekend (The weekday is from Monday to Friday and the weekend is Saturday and Sunday)
rating: Rating given by the customer out of 5
food_preparation_time: Time (in minutes) taken by the restaurant to prepare the food. 
  This is calculated by taking the difference between the timestamps of the restaurant's order confirmation and the delivery person's pick-up confirmation.
delivery_time: Time (in minutes) taken by the delivery person to deliver the food package. 
  This is calculated by taking the difference between the timestamps of the delivery person's pick-up confirmation and drop-off information
