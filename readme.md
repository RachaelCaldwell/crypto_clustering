# crypto_clustering_challenge
The Module 19 Challenge Python and unsupervised learning to predict if cryptocurrencies are affected by 24-hour or 7-day price changes.

**Requirements**<br>

***Find the Best Value for k by Using the Original Data***
- Code the elbow method algorithm to find the best value for k. Use a range from 1 to 11.
- To visually identify the optimal value for k, plot a line chart of all the inertia values computed with the different values of k. <br>

![image](https://github.com/RachaelCaldwell/crypto_clustering/blob/main/Resources/elbow_original.png?raw=true)
- Cluster the Cryptocurrencies with K-Means by Using the Original Data
- Initialize the K-means model with four clusters by using the best value for k.
- Fit the K-means model by using the original data.
- Predict the clusters for grouping the cryptocurrencies by using the original data. Review the resulting array of cluster values.
- Create a copy of the original data, and then add a new column of the predicted clusters.
- Using hvPlot, create a scatter plot by setting x="price_change_percentage_24h" and y="price_change_percentage_7d". Color the graph points with the labels that you found by using K-means. Then add the crypto name to the hover_cols parameter to identify the cryptocurrency that each data point represents.

***Optimize the Clusters with Principal Component Analysis***
- Create a PCA model instance, and set n_components=3.
- Use the PCA model to reduce the features to three principal components. Then review the first five rows of the DataFrame.
- Get the explained variance to determine how much information can be attributed to each principal component.
- Create a new DataFrame with the PCA data. Be sure to set the coin_id index from the original DataFrame as the index for the new DataFrame. Review the resulting DataFrame.
- Find the Best Value for k by Using the PCA Data
- Code the elbow method algorithm, and use the PCA data to find the best value for k. Use a range from 1 to 11.
- To visually identify the optimal value for k, plot a line chart of all the inertia values computed with the different values of k.
- Cluster the Cryptocurrencies with K-means by Using the PCA Data
- Initialize the K-means model with four clusters by using the best value for k.
- Fit the K-means model by using the PCA data.
- Predict the clusters for grouping the cryptocurrencies by using the PCA data. Review the resulting array of cluster values.
- Create a copy of the DataFrame with the PCA data, and then add a new column to store the predicted clusters.
- Using hvPlot, create a scatter plot by setting x="PC1" and y="PC2". Color the graph points with the labels that you found by using K-means. Then add the crypto name to the hover_cols parameter to identify the cryptocurrency that each data point represents.

***Visualize and Compare the Results***
- Create a composite plot by using hvPlot and the plus sign (+) operator to compare the elbow curve that you created from the original data with the one that you created from the PCA data.
- Create a composite plot by using hvPlot and the plus (+) operator to compare the cryptocurrency clusters that resulted from using the original data with those that resulted from the PCA data. 
