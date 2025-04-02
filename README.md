# Exploratory Data Analysis

## **Problem statement**
In New York City, many people use the online food delivery service, Food Hub, to order meals from their favorite restaurants, all through a single smartphone.


## **Objective** 
The objective is to analyze the data from online orders and gain a clear understanding of customer demand for different restaurants, which will help Food Hub improve its customer experience.

## **Techniques/tools utilized and achievements**
✅Exploratory Data Analysis (EDA) to answer questions that help the company to improve the business (identification of the top restaurants, etc), using Python.

✅Exploration of variables: univariate analysis (distributions), multivariate analysis (relationship between the variables).

✅Determination of the factors that affect rating and delivery time, as well as the nature of their effect.

## **Data Description**
The data contains the different data related to a food order. The detailed data dictionary is given below.

* order_id: Unique ID of the order
* customer_id: ID of the customer who ordered the food
* restaurant_name: Name of the restaurant
* cuisine_type: Cuisine ordered by the customer
* cost: Cost of the order
* day_of_the_week: Indicates whether the order is placed on a weekday or weekend (The weekday is from Monday to Friday and the weekend is Saturday and Sunday)
* rating: Rating given by the customer out of 5
* food_preparation_time: Time (in minutes) taken by the restaurant to prepare the food. 
  This is calculated by taking the difference between the timestamps of the restaurant's order confirmation and the delivery person's pick-up confirmation.
* delivery_time: Time (in minutes) taken by the delivery person to deliver the food package. 
  This is calculated by taking the difference between the timestamps of the delivery person's pick-up confirmation and drop-off information


## **Overall conclusions and project impact** 
☑️The rating is influenced by the type of cuisine, the day of the week, and the delivery time, but it is primarily determined by the type of cuisine and the day of the week.

☑️The insights into the most popular cuisine types, top restaurants, and days with the highest demand are essential for enhancing the customer experience.

☑️The raw data show several quality issues, primarily with the 'rating' and 'day_of_the_week' variables, which hinder the ability to gain better insights. Improving data recording would facilitate more effective analysis in the future.

☑️Once data recording is improved, a machine learning model can be used to accurately predict the number of orders per day, helping optimize delivery times.


# Complete script (google colab): 
FDS_PROJECT_LearnerNotebook_FullCode.ipynb

