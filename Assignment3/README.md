# ML Assignment 3

This assignment utilizes an unsupervised learning model and KMeans to cluster text data on food recalls (because of food poisoning outbreaks) - specifically descriptions of the reason (specific food items) for the recall. I made some additional changes to the feature set and data processing section to improve clustering efforts:
- Stop words were removed
- Words present in 90% or more of descriptions were removed
- ASCII accents are removed
- Limited each product description to the first 100 characters

## Elbow Plot
First, I used an elbow plot to try to identify the ideal number of clusters. It was hard to articulate a clear elbow from the plot generated. There's a point around 10 clusters and 20 clusters that could potentially be *the* elbow. I moved forward exploring how the clusters looked in silhouette plots to dive further.

![image](https://user-images.githubusercontent.com/17213588/235833843-60ea3ae0-2946-46a9-946d-6294a37fc941.png)

## Silhouette Plot
Based on the silhouette plots, the cluster of 25 had the best average coefficient. This seems like it may be too many specialized clusters - it may be easier to understand with a smaller amount of broader food group clusters. The next best average coefficient was for 5 clusters. However, this amount of clusters yielded a large cluster that seems to be mostly incorrect.

![image](https://user-images.githubusercontent.com/17213588/235833956-ef451604-b3da-4ddc-bda8-352c6fc7da37.png)

![image](https://user-images.githubusercontent.com/17213588/235834192-b2f51214-6c67-4a58-9e97-ca6e31b642e6.png)
