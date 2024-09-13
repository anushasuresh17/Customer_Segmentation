# Customer Segmentation using K-Means Clustering

In this project, I performed customer segmentation using the K-Means clustering algorithm. Customer segmentation is a key strategy used by businesses to divide a customer base into distinct groups to tailor marketing efforts, improve user experience, and drive business growth. By grouping customers based on their purchasing behavior and demographic data, companies can offer personalized services and products to meet the specific needs of each segment.

Dataset Overview: The dataset includes the following features:

Customer ID: Unique identifier for each customer.
Age, Gender: Demographic data of the customer.
Item Purchased, Category, Purchase Amount (USD): Transactional data including products and the amount spent.
Location, Size, Color, Season: Details about the products purchased.
Review Rating: Customer feedback in terms of ratings.
Subscription Status, Shipping Type, Discount Applied, Promo Code Used: Information about customer engagement and incentives.
Previous Purchases, Payment Method, Frequency of Purchases: Insights into customer behavior and loyalty.
Steps Performed:

Data Preprocessing:

Handling Missing Data: Missing values were filled or removed as necessary.
Feature Scaling: Standardized the data to bring all features to the same scale, which is crucial for distance-based algorithms like K-Means.
Encoding Categorical Variables: Converted categorical variables (e.g., Gender, Payment Method) into numerical values using one-hot encoding.
Feature Selection:

Based on the data, I chose relevant features such as Age, Purchase Amount, Review Rating, Previous Purchases, and Frequency of Purchases to segment the customers.

Optimal Number of Clusters:

Elbow Method: Used the elbow method to determine the optimal number of clusters (k) by plotting the sum of squared distances from the cluster center.

Implemented the K-Means clustering algorithm using Python's sklearn library.
Clusters were created based on the customer attributes to identify different segments of customers.

Results:

2D Model of Segmentation: Visualized the clusters in two dimensions using principal component analysis (PCA) to reduce the number of features.
3D Model Segmentation: Extended the visualization into 3D to capture more variance in the data.
Pairplot: Generated pairplots to explore the relationships between different features for each cluster.
Visualizations:

2D and 3D visualizations of the clustered data helped identify distinct customer segments, providing actionable insights for targeted marketing.
The pairplot revealed clear trends in the data, showing how different customer segments behave in terms of purchasing patterns, age, and review ratings.

Visualizations:

2D and 3D visualizations of the clustered data helped identify distinct customer segments, providing actionable insights for targeted marketing.
The pairplot revealed clear trends in the data, showing how different customer segments behave in terms of purchasing patterns, age, and review ratings.

Conclusions
Cluster 0

Purchase Amount(USD):

This group has the highest average purchase amount(compared to the other clusters), though the difference is minimal.
Frequenct of purchases:

Customers in this segment make the fewest purchase on average, indicating they might be less engaged or more occasional buyers
Review rating:

The average review rating is slightly lower than the other clusters, which could indicate slightly lower customer satisfaction
Discount Applied:

This group benefits from a lower proportion of discounts compared to the other clusters, possibly indicating they are less price-sensitive.
Cluster 1

Purchase Amount(USD):

Customers in this group spend less per purchase on average compared to Cluster 0
Frequency of purchases:

These customers purchase more frequently than cluster 0, suggeting moderate engagement.
Review rating:

Their average rating is slightly higher than cluster 0, indicating somewhat higher satisfaction
Cluster 2

Purchase Amount(USD):

The average purchase amount is comparable to cluster 1, though slightly higher
Frequency of purchases:

This is the most engaged customer segement by far, with a significantly higher frequency of purchases, suggesting these are repeat customers or brand loyalists.
Review Rating:

Customers in this segement have the highest average review rating, suggesting higher satisfaction with their purchases.
Discount applied:

Discounts are applied frequently in this cluster, but not as much as in cluster 1. This suggests that these customers may be more willing to pay full price while still using discounts on occasion.
Cluster 0 - represents occasional buyers who tend to make fewer purchases and are less influenced by discounts. They also give slightly lower review ratings, indicating they may need more attention to improve their engagement and satisfaction

Cluster 1 - represents moderately frequent buyers who are price-sensitive and more likely to use discounts. Their satisfaction levels are average, but their purchase frequency is higher than cluster 0.

Cluster 2 - represents highly engaged, loyal customers who make frequent purchases and provide the best review ratings. They are also somewhat price-sensitive, using discounts regulary but not overwhelmingly so.


Recommendations
For cluster 0 - Want to focus on increasing engagement through personalized marketing and incentives to drive more purchases

For Cluster 1 - Offering more targeted discount offers and loyalty rewards could help maintain their engagement and increase satisfaction

For Cluster 2 - These customers are higlhy loyal, so maintaining their satisfaction through premium services or exclusive offers (not necessarily discounts) could strengthemn their loyalty further.
