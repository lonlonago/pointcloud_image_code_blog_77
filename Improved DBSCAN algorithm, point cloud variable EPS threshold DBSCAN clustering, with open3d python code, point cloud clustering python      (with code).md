The traditional DBSCAN algorithm has been improved.

The clustering radius adaptively changes with the scan distance.

For long-distance obstacles, the clustering effect of point clouds is improved.

The experimental results show that the proposed method is suitable for obstacles of different distances

It can achieve good clustering.

Comparison renderings:

The density of laser point cloud data is negatively correlated with the scanning distance. The closer the scanning distance, the denser the point cloud data.

The farther the scanning distance, the sparser the point cloud data, and the DBSCAN algorithm is more sensitive to the difference in data density and clustering spacing.

It mainly relies on the debugging of eps distance parameters, and the clustering effect is good when the data is evenly distributed.

However, the clustering effect is poor when the data distribution is uneven, and different parameters have a significant impact on the final clustering effect.

Aiming at the problems of large amount and uneven distribution of laser point cloud data, the traditional DBSCAN algorithm

Improved parameter input method. DBSCAN algorithm is very sensitive to parameters eps and MinPts.

When the point cloud data is unevenly distributed and the cluster spacing varies greatly, it is difficult to choose an appropriate parameter value

This allows for good clustering at different distances.

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574673983
  ```  
