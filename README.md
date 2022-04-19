# Multinomial Logit Model Based Optimal Assortment on Customer Segmentation
OVERVIEW:

Finding and maintaining the optimal assortment of products to sell in stores has always been at the core of a retailer’s commercial activity. Retailers who get the assortment right enjoy more sales, higher gross margins, leaner operations, and most importantly, more loyal customers. On the other hand, a deeper understanding of customer segments has validated the value of focussing on different types of customers and can guide firms toward more effective ways to market products and develop strategy specifically. In particular for the online marketplace, the extensive data provides the convenience for data analysis to achieve the business goal of the company.


DATA AND MOTIVATION:

The dataset we will be working with is provided by Expedia as part of a Kaggle competition. It gives the results of search queries for hotels on Expedia. The data set contains the customers’ input for each query and its corresponding displayed hotels. Besides the general assortment optimization on all customers, we segment the customers to groups by their input of search query: Booking window, the number of adults, the number of children, the number of rooms the customer and lastly an indicator of whether the customer is looking for a Saturday night booking. Then, as a new customer comes in, we can effectively
categorize him/she/them with their query information and provide them with a specific assortment. As in the figure on the right, a shallow statistics of search with booking group by number of adults and kids from data.csv, we notice that given the historical data, the need and revenue from different types of customers vary. There are a high number of searches for two adults and a single adult, while the search query with adults and kids seems to have a higher average final price, 151 for two adults, 1 kid and 144 for 3 adults and 2 kids.


METHODS:
 
To achieve the goal of optimizing the overall expected revenue, we plan to divide customers into several groups and solve for the Multinomial Logit Model to find the optimal assortment given the set of hotels from data1.csv. We would have customer segments like:
1. Trip with a single adult and without kids: Usually considered a business trip.
2. Trip with two adults and without kids: Usually considered a couple trip.
3. Trip with three or more adults and without kids: Usually considered a group of friends trip. 4. Trip with adults and kids: Usually considered a family trip.
We will compare the result expected revenue with and without the customer segmentation to evaluate the assortment and segmentation strategy.
Furthermore, we will dig deeper into the different types of customers to analyze their sensitivity to features of the hotel by evaluating the preference weights under the multinomial logit model. More specifically, we would focus on the features of price and promotion and build a price model to determine the new display price and or whether to offer promotion given the assortment from the previous part of work.
