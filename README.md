# Credit Card Customer Segmentation using K-Means Clustering

This project performs customer segmentation on credit card data using the K-Means clustering algorithm. The goal is to identify distinct customer groups based on their spending behavior and credit limits.

## Dataset

The dataset used in this project is `CC GENERAL.csv`, which contains information about credit card customers, including their balance, purchase history, credit limits, and other relevant features.

## Project Structure

credit-card-clustering/
├── CC GENERAL.csv        # The credit card dataset
├── credit_card_clustering.py # Python script for clustering
├── README.md             # Project documentation 

## Dependencies

* Python 3.x
* pandas
* scikit-learn (sklearn)
* numpy

The script will:

Load the CC GENERAL.csv dataset.
Select relevant features (BALANCE, PURCHASES, CREDIT_LIMIT).
Scale the data using MinMaxScaler.
Apply K-Means clustering with 5 clusters.
Add the cluster labels to the original DataFrame as a new column named CREDIT_CARD_SEGMENTS.
Print the first few rows of the updated DataFrame.

View the Results:

The script will print the first few rows of the DataFrame, showing the assigned cluster labels for each customer. You can further analyze the clusters to understand the characteristics of each customer segment.

## Clustering Methodology
#Feature Selection: The project focuses on BALANCE, PURCHASES, and CREDIT_LIMIT as key features for customer segmentation.
Data Scaling: MinMaxScaler is used to scale the features to a range of 0 to 1, ensuring that features with larger ranges do not dominate the clustering process.
K-Means Clustering: The K-Means algorithm is used to group customers into 5 distinct clusters. The number of clusters (5) was chosen arbitrarily, and further analysis could be conducted to determine the optimal number of clusters using methods like the Elbow method or silhouette score.
Cluster Interpretation: The resulting clusters can be analyzed to identify customer segments with different spending behaviors and credit limits. For example, some clusters might represent high-spending customers with high credit limits, while others might represent low-spending customers with lower credit limits.

## Future Improvements
Optimal Number of Clusters: Determine the optimal number of clusters using the Elbow method or silhouette score.
Feature Engineering: Explore additional features or create new features to improve the clustering results.
Cluster Visualization: Visualize the clusters using scatter plots or other visualization techniques to better understand the customer segments.
Cluster Analysis: Conduct a more in-depth analysis of the clusters to identify key characteristics and develop targeted marketing strategies.
Other Clustering Algorithms: Test other clustering algorithms, such as DBSCAN or hierarchical clustering, to compare results.
