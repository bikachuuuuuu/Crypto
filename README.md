# Crypto

## Overview 

The purpose of this analysis is to create a report that includes what cryptocurrencies are on the trading market, and how they could be grouped to create a classification system.

## Results

To conduct this analysis, we had to preprocess the data to prepare it for Principal Component Analysis (PCA). PCA is a technique where we can reduce the dimensionality of a dataset. For our purposes, we reduced the dimensionality of the dataset to three principal components.

Screenshot 2022-10-14 at 15-25-57 crypto_clustering - Jupyter Notebook

Afterward, we used the PCA dataset to create an Elbow Curve. Elbow Curves are utilized in determining the K value, where K = how many clusters there will be for clustering.

Screenshot 2022-10-14 at 15-29-16 crypto_clustering - Jupyter Notebook

To determine the K value, we look to where there is a drastic change in the direction of the curve. In the chart above, we see that the drastic change occurs at K = 4. Therefore, we've determined our K value is 4.

After finding the K value, we initial the K-Means model and predict the clusters. With this prediction, along with the cryptocurrencies features, we created a 3D visualization of the results.

Screenshot 2022-10-14 at 15-32-33 crypto_clustering - Jupyter Notebook

When the user hovers the mouse over a point, the point will provide information regarding:
- Name of Coin
- Data of each Principal Component
- Algorithm Used

As another means of visualizing the data, we also compared the number of total coins mined and the total coin supply.

Screenshot 2022-10-14 at 15-34-48 crypto_clustering - Jupyter Notebook

When the user hovers the mouse over a point, the point will provide information regarding:
- Name of Coin
- Total Coins Mined
- Total Coin Supply
