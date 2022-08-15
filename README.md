# Crypto Investments Analysis

The purpose of this project is to cluster the cryptocurrencies from data in a CSV file by their performance in different time periods. 

All of the necessary dependencies were imported.

The CSV file was imported to read the data.

By forming the Elbow Curve, the best k-value was found to cluster the original data. The k-value was equal to 4.

Using the K-Value, the K-means model was initialized, fitted with the original data and predicted the clusters for grouping the cryptocurrencies by using the original data.

An scatter hvplot was then created to visualize the segmentation of the cryptocurrencies from the original data into clusters.

Wondering how the results would differ using the PCA method to reduce the features of the original data, a PCA model was created.

The PCA model optimized the original data into three features.

It was found that the total explained variance of the three principal components was 88.81%.
A new DataFrame was formed using the new PCA data.

Using the new PCA data, the best k-value was found by forming the Elbow Curve.

Oddly enough, the k-value was found to be 4, similar to the k-value of the original data.

Using the K-Value, the K-means model was initialized, fitted with the PCA data and predicted the clusters for grouping the cryptocurrencies by using the PCA data.

An scatter hvplot was then created to visualize the segmentation of the cryptocurrencies from the PCA data into clusters.

Then the two Elbow Curves and the two scatter hvplots were compared side by side respectively.

The conclusion we found was that the k-values were the same for both the original data and the optimized PCA data.

Both scatter plots also showed that the 4 clusters segmented the cryptocurrencies similarly and clearly.