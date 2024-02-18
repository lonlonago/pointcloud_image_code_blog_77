You need to find the index of the closest point pair between point clouds A and B 

 Open3D does not have a function that directly returns a point-to-distance index, but you can obtain a point-to-distance index by following these steps: 

 Use the compute_point_cloud_distance function to calculate the distance between A and B and set the distance threshold, setting the distance less than the threshold to 0 and the distance greater than or equal to the threshold to infinity. 

 2. Use the argmin function to find the smallest value of each row in the distance matrix and its corresponding column index, which is the index of the nearest point in the target point cloud B. 

 3. Combine the distance matrix and the column index of the nearest point into a point pair index matrix to obtain the shortest distance between all point pairs and their corresponding point indexes. 

 Here is the example code: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574663263
  ```  
 The output is an (N, 2) array representing the index of the closest pair of points between A and B. For example, the first row represents the closest distance between point 0 in A and point 75 in B. 

