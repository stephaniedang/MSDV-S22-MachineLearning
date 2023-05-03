# ML Assignment 3

This assignment utilizes an unsupervised learning model and KMeans to cluster text data on food recalls (because of food poisoning outbreaks) - specifically descriptions of the reason (specific food items) for the recall. I made some additional changes to the feature set and data processing section to improve clustering efforts:
- Stop words were removed
- Words present in 90% or more of descriptions were removed
- ASCII accents are removed
- Limited each product description to the first 100 characters

## Elbow Plot
First, I used an elbow plot to try to identify the ideal number of clusters. It was hard to articulate a clear elbow from the plot generated. There's a point around 10 clusters and 20 clusters that could potentially be *the* elbow. I moved forward exploring how the clusters looked in silhouette plots to dive further.

![image](https://user-images.githubusercontent.com/17213588/235832260-f20e4df8-f6ed-433e-9d73-ddf26417b923.png)

## Silhouette Plot
