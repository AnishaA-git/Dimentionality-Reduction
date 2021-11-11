# Dimentionality-Reduction

## Colab Link: https://colab.research.google.com/drive/1H3v_0Ivo7J1S_78jZAG8uCypXX8O98Fk#scrollTo=95Onv8IJEzaB

### 2D Dimentionality Reduction
1. PCA - https://github.com/AnishaA-git/Dimentionality-Reduction/blob/master/2D%20and%203D%20images/2D%20PCA%20with%204%20components.png
2. SVD - https://github.com/AnishaA-git/Dimentionality-Reduction/blob/master/2D%20and%203D%20images/2D%20SVD.png
3. LLE - https://github.com/AnishaA-git/Dimentionality-Reduction/blob/master/2D%20and%203D%20images/2D%20LLE%20for%204%20Components.png
4. T-SNE - https://github.com/AnishaA-git/Dimentionality-Reduction/blob/master/2D%20and%203D%20images/2D%20T-SNE%20for%203%20Components.png

### 3D Dimentionality Reduction
1. PCA 3components - https://github.com/AnishaA-git/Dimentionality-Reduction/blob/master/2D%20and%203D%20images/3D%20PCA%20with%203%20components.png
2. PCA 4components - https://github.com/AnishaA-git/Dimentionality-Reduction/blob/master/2D%20and%203D%20images/3D%20PCA%20with%204%20components.png
3. PCA 5components - https://github.com/AnishaA-git/Dimentionality-Reduction/blob/master/2D%20and%203D%20images/3D%20PCA%20with%205%20components.png
4. LLE 3components - https://github.com/AnishaA-git/Dimentionality-Reduction/blob/master/2D%20and%203D%20images/3D%20LLE%20for%203%20Components.png
5. LLE 4components - https://github.com/AnishaA-git/Dimentionality-Reduction/blob/master/2D%20and%203D%20images/3D%20LLE%20for%204%20Components.png
6. LLE 5components - https://github.com/AnishaA-git/Dimentionality-Reduction/blob/master/2D%20and%203D%20images/3D%20LLE%20for%205%20Components.png
7. T-SNE 3components - https://github.com/AnishaA-git/Dimentionality-Reduction/blob/master/2D%20and%203D%20images/3D%20T-SNE%20for%203%20Components.png

### Execution Time for each Technique, for both Tabular and Image dataset
![execution-time](https://user-images.githubusercontent.com/70603792/141213413-2f61054b-085e-436d-b2f1-372ce4af91d2.png)

1. We can see that image dataset takes more time for the above techniques as compared with tabular dataset.
2. Also, among the techniques, PCA is the most efficient technique for dimentionality reduction as it takes least amount of time in both datasets.
3. UMAP takes the longest time for the reduction of dimentionality.

In terms of plotting or varience %:
1. PCA was not able to do such a good job in differentiating the faces in image dataset and points in tabular dataset. The main drawback of PCA is that it is highly influenced by outliers present in the data. PCA is a linear projection, which means it can’t capture non-linear dependencies, its goal is to find the directions (the so-called principal components) that maximize the variance in a dataset.
2. T-SNE does a better job (it tries to preserve topology neighbourhood structure) as compared to PCA when it comes to visualising the different patterns of the clusters. Similar labels are clustered together, even though there are big agglomerates of data points on top of each other, certainly not good enough to expect a clustering algorithm to perform well.
3. UMAP outperformed T-SNE and PCA, if we look at the 2d and 3d plot, we can see mini-clusters that are being separated well. It is very effective for visualizing clusters or groups of data points and their relative proximities. However, for this use case certainly not good enough to expect a clustering algorithm to distinguish the patterns.
4. Overall, when we see the 2D and 3D plotting of tabular data, it is very clear that T-SNE is the best technique among PCA, SVD and LLE.
