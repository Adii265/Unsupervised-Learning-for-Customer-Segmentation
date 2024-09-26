# Unsupervised-Learning-for-Customer-Segmentation


Algorithm Used: KMeans

To find the optimal number of clusters(Value of k): Elbow Method


Full course on: https://www.coursera.org/projects/machine-learning-for-customer-segmentation

My certificate: https://www.coursera.org/account/accomplishments/certificate/S42CVPSNE7BY

## DBSCAN Performance Metrics

| DBSCAN Model | Calinski-Harabasz Index | Davies-Bouldin Index | Silhouette Score |
|--------------|-------------------------|----------------------|------------------|
| DBSCAN2 (eps=0.2, min_samples=10)  | 6.898 | 1.393 | -0.4428 |
| DBSCAN3 (eps=0.2, min_samples=15)  | 12.675 | 1.536 | -0.3662 |
| DBSCAN4 (eps=0.2, min_samples=20)  | 19.283 | 1.559 | -0.2645 |
| DBSCAN5 (eps=0.4, min_samples=5)   | 23.289 | 1.553 | -0.2472 |
| DBSCAN6 (eps=0.4, min_samples=10)  | 22.391 | 1.421 | -0.4039 |
| DBSCAN7 (eps=0.4, min_samples=15)  | 31.466 | 1.535 | -0.3652 |
| DBSCAN8 (eps=0.4, min_samples=20)  | 36.508 | 1.554 | -0.3566 |
| DBSCAN9 (eps=0.6, min_samples=5)   | 34.876 | 1.555 | -0.3504 |
| DBSCAN10 (eps=0.6, min_samples=10) | 24.445 | 1.398 | -0.4771 |
| DBSCAN11 (eps=0.6, min_samples=15) | 73.362 | 1.620 | -0.3097 |
| DBSCAN12 (eps=0.6, min_samples=20) | 119.663 | 1.776 | -0.1580 |


## Spectral Clustering Performance Metrics

| Spectral Model | Calinski-Harabasz Index | Davies-Bouldin Index | Silhouette Score |
|----------------|-------------------------|----------------------|------------------|
| Spectral2 (n_clusters=3, n_neighbors=10)  | 166.039  | 1.990 | -0.1072 |
| Spectral3 (n_clusters=4, n_neighbors=10)  | 1542.273 | 2.002 |  0.1830 |
| Spectral4 (n_clusters=5, n_neighbors=10)  | 1265.731 | 1.732 |  0.1590 |
| Spectral5 (n_clusters=6, n_neighbors=10)  | 986.806  | 1.686 |  0.0183 |
| Spectral6 (n_clusters=7, n_neighbors=10)  | 855.469  | 1.542 |  0.0260 |
| Spectral7 (n_clusters=8, n_neighbors=10)  | 675.021  | 1.624 | -0.0487 |
| Spectral8 (n_clusters=9, n_neighbors=10)  | 593.180  | 1.537 | -0.0477 |
| Spectral9 (n_clusters=10, n_neighbors=10) | 715.525  | 1.507 | -0.0389 |
| Spectral10 (n_clusters=2, n_neighbors=5)  | 740.453  | 1.340 | -0.0146 |
| Spectral11 (n_clusters=3, n_neighbors=5)  | 754.815  | 1.375 |  0.0048 |
| Spectral12 (n_clusters=4, n_neighbors=5)  | 1469.224 | 2.027 |  0.1736 |
| Spectral13 (n_clusters=5, n_neighbors=5)  | 769.277  | 1.940 | -0.1508 |
| Spectral14 (n_clusters=6, n_neighbors=5)  | 832.167  | 1.715 | -0.0970 |
| Spectral15 (n_clusters=7, n_neighbors=5)  | 692.688  | 1.558 | -0.0942 |
| Spectral16 (n_clusters=8, n_neighbors=5)  | 672.553  | 1.531 | -0.0749 |
| Spectral17 (n_clusters=9, n_neighbors=5)  | 626.054  | 1.413 | -0.0654 |
| Spectral18 (n_clusters=10, n_neighbors=5) | 715.024  | 1.433 | -0.0423 |
| Spectral3 (n_clusters=4, n_neighbors=10)  | 1542.273 | 1.340 |  0.1830 |


## GMM Performance Metrics

| GMM Model | Calinski-Harabasz Index | Davies-Bouldin Index | Silhouette Score |
|-----------|-------------------------|----------------------|------------------|
| GMM1 (n_components=2)  | 704.522 | 1.348 | -0.0322 |
| GMM2 (n_components=3)  | 739.907 | 1.391 | -0.0013 |
| GMM3 (n_components=4)  | 1247.018 | 2.285 | 0.1855 |
| GMM4 (n_components=5)  | 907.395 | 2.652 | 0.1124 |
| GMM5 (n_components=6)  | 841.979 | 2.408 | 0.1021 |
| GMM6 (n_components=7)  | 699.449 | 2.355 | 0.0767 |
| GMM7 (n_components=8)  | 552.724 | 3.384 | 0.0452 |
| GMM8 (n_components=9)  | 503.824 | 2.821 | 0.0290 |
| GMM9 (n_components=10) | 520.905 | 2.781 | 0.0331 |
| GMM10 (n_components=11) | 407.872 | 3.326 | 0.0280 |
| GMM11 (n_components=12) | 381.895 | 3.006 | 0.0111 |

