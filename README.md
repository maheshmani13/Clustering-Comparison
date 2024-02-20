# Clustering Using Pycaret and Comparing Different PreProcessing Techniques

## Introduction

In this assignment , we have performed three types of clustering on the dataset , and we have compared the performance of clustering algorithms by using different preprocessing techniques and different cluster numbers.

Three type of clustering methods used are :
1. KMeans Clustering
2. Herireichal Clustering
3. MeanShift Clustering


## Dataset

The dataset used here is **Anuran Calls (MFCCs)**. 
We have taken it from UCI datset library.

This dataset has Acoustic features extracted from syllables of anuran (frogs) calls, including the family, the genus, and the species labels. 

Number of Instances (records in our data set): 7195

Number of Attributes (fields within each record): 24 + 1 (ID)

This dataset was used in several classifications tasks related to the challenge of anuran species recognition through their calls. It is a multilabel dataset with three columns of labels. This dataset was created segmenting 60 audio records belonging to 4 different families, 8 genus, and 10 species. Each audio corresponds to one specimen (an individual frog), the record ID is also included as an extra column.


## Metrics Used

1. **Silhouette Score** : It is a metric to evaluate the performance of clustering algorithm. It uses compactness of individual clusters(intra cluster distance) and separation amongst clusters (inter cluster distance) to measure an overall representative score of how well our clustering algorithm has performed.

This score for one sample is calculated as follows and then averaged over all samples: 
![](https://github.com/maheshmani13/Clustering-Comparison/blob/main/Metric%20Formulas/sillhoutte.png)

2. **Calinski-Harabasz Score** : The score is defined as ratio of the sum of between-cluster dispersion and of within-cluster dispersion.

![](https://github.com/maheshmani13/Clustering-Comparison/blob/main/Metric%20Formulas/Calinski.png)

3. **Davies-Bouldin** : The Davies-Bouldin Index is a validation metric that is used to evaluate clustering models. It is calculated as the average similarity measure of each cluster with the cluster most similar to it. In this context, similarity is defined as the ratio between inter-cluster and intra-cluster distances. As such, this index ranks well-separated clusters with less dispersion as having a better score.

![](https://github.com/maheshmani13/Clustering-Comparison/blob/main/Metric%20Formulas/Davies-Bouldin.png)


## Results Obtained

![](https://github.com/maheshmani13/Clustering-Comparison/blob/main/Results/Kmeans.png)

![](https://github.com/maheshmani13/Clustering-Comparison/blob/main/Results/Hierarchical.png)

![](https://github.com/maheshmani13/Clustering-Comparison/blob/main/Results/Mean%20Shift.png)
