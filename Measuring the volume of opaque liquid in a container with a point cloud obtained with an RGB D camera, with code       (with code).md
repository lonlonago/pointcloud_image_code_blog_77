 In order to measure volume effectively with this method, it is first necessary to obtain point clouds in the lower plane (the ground) and the upper plane (the top surface of the liquid).

In addition, these point clouds must be located in the plane because the points in them have the same z-coordinate. Therefore, it is possible to first need to align with the plane estimator (MSAC) and rotate in space.

##area

In order to calculate the area of the top plane point cloud, the convex hull of the curved surface is first obtained, and then the area is obtained by applying the Gaussian area formula using the points that form the convex hull.

##height

To obtain the height of the liquid in the container, a robust method for removing outliers is first applied, and then the height is obtained by using the median difference between the lower and upper z coordinates.

Volume is the product between area and height.

Various opaque liquids under different conditions were tested. In all cases, the error between the actual volume and the obtained volume was less than 10%. 

 The code is as follows: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574638919
  ```  
  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574638919
  ```  
  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574638919
  ```  
