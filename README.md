# deep-learning-practice
Yonsei University Summer 2023 Research Internship


## K-means clustering practice 
##### Yonsei University Deep Learning 4-2
##### July 4th, 2023

####  Unsupervised learning algorithm: clustering
- detect innate patterns in unlabeled data
- it is useful when you don't know what you're looking for
- requires data, but not the labels
- results may not make sense

#### What is K-means clustering?
- Clustering: group together "similar" (option: small squared Euclidean distance) instances
- K: number of clusters. user-defined hyper-parameter
- it's non-deterministic (output changes depending on input)
- it always converges, but not necessarily to an optimal solution

#### Algorithm:
1) pick k random points as cluster centers
2) assign each example data point to the mean cluster that is closest to it using Euclidean distance
3) update cluster center using the mean of points in each cluster
   
#### Elbow Method:
- used to figure out how many clusters we should use
- WCSS = within-cluster sum of squares = distance between points in cluster
- want to minimize WSS, such that WCSS is low but the clusters are small enough to interpret
