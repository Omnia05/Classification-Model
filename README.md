# Classification Model Using K-Means Clustering

The Classification Model is a Supervised Learning technique that is used to identify the category of new observations on the basis of training data. In classification, a program learns from the given dataset or observations and then classifies an observation into a number of groups. In this project, we implement the K-Means clustering technique from scratch to perform clustering analysis on pincode data from Telangana, India.

## K-Means Clustering

K means clustering, assigns data points to one of the K clusters depending on their distance from the center of the clusters.  
It starts by randomly assigning the clusters centroid in the space.  
Then each data point is assigned to one of the cluster based on its distance from the centroid of the cluster.  
After assigning each point to one of the cluster, new cluster centroids are assigned.  
This process runs iteratively until it finds good cluster.

### Choosing K, The Elbow Method

Elbow Method is a technique that we use to determine the number of centroids(k) to use in a k-means clustering algorithm.  In this method to determine the k-value we continuously iterate for k=1 to k=n the within-cluster sum of squares (WCSS) value and use this to plot a graph. The optimal K value is identified at the point where the graph bends like an elbow.

## Project Description

The dataset 'clustering_data.csv' contains information about various pincodes across India including their corresponding longitudes and latitudes.   
Here, we choose the state Telangana and perform the following steps:   
1. Data Filtering: Extract the entries corresponding to Telangana in the dataset. Remove any false locations and duplicates.     
2. Clustering Analysis: Implement the k-means clustering algorithm on the filtered dataset.
3. Visualization: Show the results of the pincode locations (using the latitude and longitude values) on a map.

### Results

The final map shows the plotted values of the pincode locations, resembling the shape of Telangana.  
The density of pincodes varies, indicating regions with higher population density.

## Prerequisites

Make sure to have pandas, numpy and matplotlib installed on your system.  
If not already installed, run these commands on your terminal:  
1. pip install pandas  
2. pip install numpy
3. pip install Matplotlib

## Resources

Going through the numpy and Matplotlib documentation has proven to be very useful.  
Sites like GeeksforGeeks provided a lot conceptual explanations.  

## Note

This is my first attempt at building a classification model. As a newcomer to these topics, I found this project both fun and insightful. I'm excited to explore further and improve my model.
