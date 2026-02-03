**Context**: The number of restaurants in New York is increasing day by day. Lots of students and busy professionals rely on those restaurants due to their hectic lifestyles. Online food delivery service is a great option for them. It provides them with good food from their favorite restaurants. A food aggregator company FoodHub offers access to multiple restaurants through a single smartphone app.
The app allows the restaurants to receive a direct online order from a customer. The app assigns a delivery person from the company to pick up the order after it is confirmed by the restaurant. The delivery person then uses the map to reach the restaurant and waits for the food package. Once the food package is handed over to the delivery person, he/she confirms the pick-up in the app and travels to the customer's location to deliver the food. The delivery person confirms the drop-off in the app after delivering the food package to the customer. The customer can rate the order in the app. The food aggregator earns money by collecting a fixed margin of the delivery order from the restaurants.

**Objective**: The food aggregator company has stored the data of the different orders made by the registered customers in their online portal. They want to analyze the data to get a fair idea about the demand of different restaurants which will help them in enhancing their customer experience. Suppose you are hired as a Data Scientist in this company and the Data Science team has shared some of the key questions that need to be answered. Perform the data analysis to find answers to these questions that will help the company to improve the business.

**Data Description**: The data contains the different data related to a food order. The detailed data dictionary is given below.

**Data Dictionary**
1. order_id: Unique ID of the order
2. customer_id: ID of the customer who ordered the food
3. restaurant_name: Name of the restaurant
4. cuisine_type: Cuisine ordered by the customer
5. cost: Cost of the order
6. day_of_the_week: Indicates whether the order is placed on a weekday or weekend (The weekday is from Monday to Friday and the weekend is Saturday and Sunday)
7. rating: Rating given by the customer out of 5
8. food_preparation_time: Time (in minutes) taken by the restaurant to prepare the food. This is calculated by taking the difference between the timestamps of the restaurant's order confirmation and the delivery person's pick-up confirmation.
9. delivery_time: Time (in minutes) taken by the delivery person to deliver the food package. This is calculated by taking the difference between the timestamps of the delivery person's pick-up confirmation and drop-off information

**Conclusions from the data analysis**:
1. Delivery time significantly increases during the weekday
2. The number of orders is more than 2x in the weekend compared to the weekday
3. The top 10 restaurants in terms of order volume contribute to 46.0 % of the total order amount
4. Food preparation or Delivery time bears no such effect on the cuisine or restaurant selected for ordering
5. Food preparation time and Food delivery time have a slight negative impact on Rating as the correlation is negative, but the correlation is quite weak
6. The top 5 cuisines ordered does not change much between weekday to weekend. The top five cuisines are American, Japanese, Italian, Chinese, and Mexican
7. The ticket size of the orders (order amount/#order) is the highest for French cuisine and lowest for Vietnamese cuisine
8. The ratings are quite similar across the different cuisines. But Spanish has the highest average rating, closely followed by Thai and Indian cuisines

**Recommendations**:
1. Recommend FoodHub to provide discounts to customers based on the Total order amount and not on #orders. There can be a condition applied on the minimum number of orders (say 5) to be eligible for the discount.
