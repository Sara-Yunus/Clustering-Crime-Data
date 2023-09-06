# Crime Data Clustering using both KMeans and DBSCAN

I tried my hands on clustering data using Unsupervised Learning using KMeans and Density-Based Spatial Clustering of Applications with Noise (DBSCAN). Took data in csv file format from https://data.gov/ (refer About_the_data.txt for data dictionary). I used only 1400 datapoints out of 788767 datapoints originally present. I downsized the dataset to accommodate my laptop's performance limitations.

## Process Overview 

First I used KMeans Algorithm on my dataset
* Calculated its silhouette score
* Visulaised Elbow plot to find the optimal value of k
* Visualised the clusters obtained using KMeans.

Then I used DBSCAN ALgorithm with eps=0.2 and min_samples=6
* Calculated its silhouette score
* Visualised the obtained clusters for the aforementioned values
* Found optimal values for DBSCAN paraemters eps and min_samples
* Plotted sorted k-dist graph.

## Comparative Overview
 
* Both the clustering algorithm used on this dataset gives 3 as the most favorable cluster value.
* Cluster validation is performed using silhouette score on both the KMeans and DBSCAN models. 
At the optimum parameter value, K-means algorithm has a 0.8276 silhouette score and DBSCAN algorithm has 0.8165 silhouette score.
* K-means performed better.
