# Credit Card Customer Segmentation

## Overview
This project focuses on segmenting credit card customers into distinct categories based on their spending behavior and financial activities. The analysis uses multiple clustering algorithms, including KMeans, DBScan, GMM (Gaussian Mixture Model), and Spectral Clustering, to identify different customer types. Understanding these segments can help financial institutions tailor their services and marketing strategies.

## Clustering Algorithms Used
- **KMeans**: A widely used clustering algorithm that partitions the data into K distinct clusters based on feature similarity.
- **DBScan**: A density-based clustering algorithm that identifies clusters of varying shapes and sizes based on the density of data points.
- **GMM**: A probabilistic model that assumes all data points are generated from a mixture of several Gaussian distributions, suitable for soft clustering.
- **Spectral Clustering**: Uses the eigenvalues of a similarity matrix to reduce dimensionality before applying a clustering algorithm, effective for complex cluster shapes.

## Customer Segments
Based on the analysis, the following customer segments have been identified:

### KMeans Clustering
1. **Transactors**: 
   - Paid least amount of interest charges
   - Careful with their money
   - Lowest balance and cash advance
   - Full payment percentage: 24%

2. **Revolvers**: 
   - Use credit card as a loan
   - Most lucrative sector
   - Highest balance and cash advance
   - Low purchase frequency, high cash advance frequency

3. **VIP/Prime**: 
   - High credit limit
   - High percentage of full payment: 39%

4. **Low Tenure**: 
   - Low tenure and low balance

### GMM Clustering
1. **Transactors**: Similar profile as KMeans.
2. **Revolvers**: High balance and cash advances, comparable to KMeans.
3. **VIP/Prime**: High credit limits and full payments.
4. **Low Tenure**: New customers with lower balances.

### Spectral Clustering
1. **Transactors**: Careful spenders, akin to KMeans.
2. **Revolvers**: Frequent cash advance users, matching the KMeans profile.
3. **VIP/Prime**: High spending and reliable payment behavior.
4. **Low Tenure**: Short credit history customers.

### DBScan Clustering
1. **Transactors**: Responsible credit users with minimal cash advances.
2. **Revolvers**: High balances and cash advances.
3. **VIP/Prime**: Elite users with high credit limits.
4. **Low Tenure**: Customers with shorter histories.

## Evaluation Metrics
The performance of the clustering algorithms was evaluated using the following metrics:
- **Calinski-Harabasz Index**: Higher values indicate better-defined clusters.
- **Davies-Bouldin Index**: Lower values suggest better separation between clusters.
- **Silhouette Score**: Ranges from -1 to 1, where values closer to 1 indicate better clustering.

### Clustering Results
| Algorithm | Calinski-Harabasz Index | Davies-Bouldin Index | Silhouette Score |
|-----------|-------------------------|----------------------|------------------|
| KMeans    | 1542.27                 | 1.34                 | 0.18             |
| GMM       | 1247.02                 | 2.28                 | 0.27             |
| Spectral  | 1265.73                 | 1.73                 | 0.16             |
| DBScan    | 980.80                  | 1.52                 | 0.19             |

## Installation
To run this project, ensure you have the following installed:
- Python 3.x
- Required libraries:
  ```bash
  pip install pandas numpy scikit-learn matplotlib seaborn


### Observations
- **KMeans** achieved the highest Calinski-Harabasz Index of **1542.27**, indicating well-defined clusters. However, its Davies-Bouldin Index of **1.34** suggests some overlap between clusters, with a moderate silhouette score of **0.18** indicating that some points are not well matched to their assigned clusters.
  
- **GMM** displayed a Calinski-Harabasz Index of **1247.02**, reflecting good cluster separation. Its Davies-Bouldin Index of **2.28** was the highest among all algorithms, indicating the most overlap. The Silhouette Score of **0.27** shows that many data points are closer to their own clusters compared to others.

- **Spectral Clustering** yielded a Calinski-Harabasz Index of **1265.73**, slightly lower than KMeans but still indicative of good cluster separation. The Davies-Bouldin Index of **1.73** suggests better-defined clusters than GMM, while a Silhouette Score of **0.16** implies that some points are less cohesively grouped.

- **DBScan** had the lowest Calinski-Harabasz Index of **980.80**, indicating less defined clusters. However, its Davies-Bouldin Index of **1.52** suggests relatively better separation than GMM, with a Silhouette Score of **0.19** indicating moderate clustering quality.

Overall, while KMeans and GMM provide solid clustering results, GMM's greater flexibility may allow it to capture more complex patterns in data. Spectral and DBScan offer alternative approaches, particularly useful in detecting clusters of varying shapes and densities.


**Full course on:** https://www.coursera.org/projects/machine-learning-for-customer-segmentation

**My certificate:** https://www.coursera.org/account/accomplishments/certificate/S42CVPSNE7BY
