The file with my code is found in the "Crypto-Clustering_dr" file in the "Starter_Code".

The data here examined the price changes for various cryptocurrencies within various timeframes.
In order to get clustered data, the fit and transform functions from the Standard Scaler module were used on the market data.
The ideal number of clusters was found using the elbow test, which here equals 4.
The clusters that each data point would correspond to was decided using the predict function.
A scatter plot was created, with 24 hour price changes on the x-axis and price changes over 7 days on the y-axis. Clusters 0 and 2 each seem to have only one point,
  but clusters 1 and 3 have multiple points. Both of these clusters have points that are spread out, but cluster 3 seems to be more so than cluster 1.

This process was repeated but using the PCA (principle component analysis) method, using 3 components.
4 also was found to be the ideal value for k.
The scatter plot for PCA method was made, this time clusters 0 and 3 had multiple points.
While still somewhat spread out, clusters 0 and 3 each have points that appear to be in closer proximity to each other than the Standard Scaler way.

The observation, as is also stated at the end of the notebook file, is that PCA, with a limited number of components, creates clusters whose points are closer together. With not as many aspects 
to compare to, it would make sense that there would be less differences in the variances of each of these points. The clusters themselves also appear to be closer together as well.
