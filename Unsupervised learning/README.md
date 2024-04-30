# Unsupervised Learning: K-Means vs DBSCAN, PCA


### Introduction
Unsupervised learning is a machine learning technique where only input data (X) is available without corresponding output labels. The goal is to discover patterns and structures within the data without external guidance. Key challenges include the absence of true labels for comparison of model performance.   

<p align="center">
    <img src="ML.jpeg" width="700" hight ="800">
</p>
  

### Key Concepts
- **Clustering**: Grouping data points such that those within the same group are more similar to each other than to those in other groups.  

- **Dimensionality Reduction**: Reducing the number of random variables while preserving variance in the data.
Association: Discovering rules describing portions of the data.  

- **Anomaly Detection**: Identifying rare items, events, or observations.  

### Dimensionality Reduction with PCA  

- PCA (Principle Component Analysis) is an unsupervised learning technique for reducing the number of features in a dataset while preserving variance.  
- It relies on eigenvalue decomposition and is often used as a preprocessing step before implementing supervised or unsupervised learning algorithms.  

## Clustering Algorithms


### K-Means Clustering
- **Description**: Centroid-based or partition-based clustering algorithm that partitions all points in the sample space into K groups of similarity.    
- **Algorithm**:  
  1. Randomly place K centroids, one for each cluster.  
  2. Calculate the distance of each point from each centroid.  
  3. Assign each data point to its closest centroid, forming clusters.  
  4. Recalculate the position of K centroids.  

- **Pros**: Simple and easy to implement, computationally efficient.  
- **Cons**: Sensitive to initial centroid placement, assumes spherical clusters, requires predefined K.  

### DBSCAN Clustering
- **Description**: Density-based clustering algorithm that groups points based on density in a given radius.  

- **Algorithm**:
  1. Determine the type of each point: Core, Border, or Outlier.    
  2. Connect core points and assign border points to clusters.  
  3. Eliminate outlier points.  

- **Pros**: Robust to noise and outliers, does not require predefined K.  

- **Cons**: Sensitive to parameter tuning, may struggle with varying density.  

### Comparison

- **K-Means**:  
  - Suitable for datasets with well-defined spherical clusters.  
  - Works best when clusters have similar density.  
  - Requires prior knowledge of the number of clusters.  

- **DBSCAN**:  
  - Effective for datasets with irregularly shaped clusters.  
  - Robust to noise and outliers.  
  - Automatically determines the number of clusters.  


### Conclusion  

The choice between K-Means and DBSCAN depends on the nature of the dataset and the desired outcome.
K-Means is preferred for datasets with clear clusters and known cluster count.
DBSCAN is recommended for datasets with varying cluster shapes and density, or in scenarios where noise and outliers need to be handled effectively.