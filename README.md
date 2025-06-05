# Exploratory Data Analysis (Food Hub order analysis using Python)

Complete google Collab script (Python code):
https://github.com/arincons2/ExploratoryDataAnalysis/blob/7352fedaae0187e353012ee512a4db3a1fb93a23/FDS_PROJECT_FullCode_V3c.ipynb

## **Problem statement**
In New York City, many people use the online food delivery service, Food Hub, to order meals from their favorite restaurants, all through a single smartphone.


## **Objective** 
The objective is to analyze the data from online orders and gain a clear understanding of customer demand for different restaurants, which will help Food Hub improve its customer experience. The main result is to determine the factors that affect rating, count of orders and delivery time.

## **Techniques utilized**
Exploratory Data Analysis (EDA) using Python (Google collab):

✅ Exploration, cleaning and preparation of data.

✅ Univariate analysis (countplots, histograms, boxplots) and multivariate analysis (heatmap, pairplot, covariance heatmap, multivarite countplots, etc) to determine the factors that affect rating, count of orders and delivery time.

✅ Data querying, aimed at answering questions that help the company improve the business (identification of the top restaurants, etc), using aggregation operations and Python functions.

## **Tools utilized**
✅Language: Python (Google collab)

✅ Python libraries: Numpy, Pandas, Matplotlib, Seaborn.  

## **Overall conclusions** 
From the count plots it follows that:

☑️ The count of orders is influenced by the cuisine type, restaurant name, delivery time, the day of the week, the cost and the rating. These input factors are crucial for enhancing the customer experience.

☑️ The rating depends on the cuisine type and restaurant name. 

☑️ The delivery time depends on day of the week and cuisine type. 

☑️ The demand (count of orders) is higher on weekends than on weekdays

☑️ The count of orders is increasing with the rating. This implies that the food quality has a strong influence on the demand.

☑️ The count of orders exhibits a significant decrease for delivery time higher than 30.

From the plots for rating, delivery time and cost it follows that:

☑️ The dependence of rating on cuisine type is strong, but its dependence with respect to day of week, delivery time,
food preparation time, and cost range is low. This implies that the criterion for registration of rating is straightforwardly related to food quality, and not on other variables.

☑️ The delivery time depends on the day of the week.

☑️ The dependence of delivery time on cuisine type and restaurant name is weak.

☑️ The cost of the order depends on the cuisine type, but it does not depend on day of the week (in average).

☑️ The dependence of food preparation time with cuisine type is not strong.


## **Recommendations** 
☑️ Since the count of orders exhibits a significant decrease for delivery time higher than 28 during weekdays, it is recommended to identify the corresponding restaurants or circumstances, and solve this issue. These higher delivery times occur during weekdays.

☑️ It is recommended to perform marketing campaign for the restaurants with higher demand. Also, it would be convenient to identify the three restaurants with higher demand (and higher rating) for each cuisine type, and make publicity for these. This would facilitate the people to choose apropriate foods, in special to those who haven't a certain decision.

☑️ It is recommended to use a more detailed rating, using numbers 3.0, 3.2, 3.4, .....4.6, 4.8, 5.0, instead of the current numbers used (3.0, 4.0, 5.0). This would lead to a better understanding of the dependence of 'rating' with respect to the different input variables.

☑️ It is recommended to use a more detailed racording of the 'day of week', specifying the exact day of the week, not the current binary category (weekend/weekday). This would allow to understand the dependence of rating and count with respect to day of the week, and also it would allow to identify the days with higher delivery time and to solve it.

☑️ After improving the recording of 'rating' and 'day_of_the_week' values, the EDA can be made again, leading to deeper conclusions and recommendations.


# Complete script (google colab script, including detailed code, insights and recommendations): 

https://github.com/arincons2/ExploratoryDataAnalysis/blob/7352fedaae0187e353012ee512a4db3a1fb93a23/FDS_PROJECT_FullCode_V3c.ipynb

https://github.com/arincons2

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

