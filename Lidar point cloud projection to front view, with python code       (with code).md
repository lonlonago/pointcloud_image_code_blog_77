According to the laser radar harness number and horizontal angle (which can also be calculated), the point cloud is projected to the front view. The effect is as follows: 

 ![avatar]( 08971c037b85042510a626d27caca040.png) 

##  Spherical projection derivation process 

 Suppose there is an m-line rotating scanning lidar, its vertical field of view FOV is divided into two parts: FOV_up and FOV_down, usually with the value of FOV_up is positive and FOV_down value is negative, so FOV = FOV_up + abs (FOV_down). The point cloud obtained by the rotation of the lidar scanning is equivalent to a hollow cylinder centered on itself. If the cylinder is unfolded, then the point cloud can be projected into an image plane, which is the distance image. 

 For an m-line lidar, m points will be obtained at a certain time of scanning. If the rotation is scanned n times, the resulting point cloud can be represented by a matrix. So how to project a 3-dimensional point cloud to a 2-dimensional distance image plane? This requires the use of spherical coordinates. 

 ![avatar]( 76a34bbd935237c5ecaf4d9841bfba70.png) 

 If the cylinder obtained by rotating and scanning the lidar in the direction of the front view in the x-axis direction is expanded, an image like this can be obtained: the coordinate origin is in the center of the image, and the ordinate of the pixel in the image is obtained by the pitch angle projection (range is [FOV_down, FOV_up]), and the abscissa is obtained by the yaw angle projection (range is). 

 ![avatar]( 764947ff2b3086b33da9fa493fa8f901.png) 

 Since the image coordinate system uses the upper left corner as the coordinate origin, the front view obtained above also needs to be transformed to move the coordinate origin to the upper left corner: 

 Projecting a 3-dimensional point cloud into a 2-dimensional image will inevitably lead to information loss. In order to minimize the information loss caused by projection, we need to choose the appropriate size of the projected image. For a 64-line lidar, the height of the projected image is generally set to 64, so how to set the width of the image? Assuming that the horizontal resolution of the lidar is 0.35 degrees, the maximum number of points produced by rotating a laser once is. In convolutional neural networks, the input feature map is generally downsampled by 2 times many times, so the width of the image needs to be set to the power of 2, which can be set to 1024 here. 

 Due to the different field angles and horizontal resolutions of different types of lidar, the size of the projected image will also be set to different values as needed. In order to adapt to these changes, yaw and pitch also need to be standardized. 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574625162
  ```  
