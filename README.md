 The program only uses a python code file, uses the socket module to communicate with the radar, and can save and read the bin data file. It is simple and easy to use 

 The code is as follows: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574645567
  ```  
 How to use the radar via port 2368: 

 ./velodyne.py read .\file_dir

 How to use the program to read saved radar data: 

 ./velodyne.py unpack .\file_path



--------------------------------------------------------------------------------

Method 3  

 You can also split the channels first, and then merge the channels after assignment to compare the consumption time and memory 

 Method 4  

 Use the mat array mat [N], and then assign values to each channel element individually 

 Method 1 - More efficient 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574611508
  ```  
 Method 2 - More elegant 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574611508
  ```  
 P.S.: It is important to note that according to the documentation, matrices created with Mat :: create () are always continuous. However, if you use Mat :: col (), Mat :: diag (), etc. to extract a portion of a matrix, or construct a matrix header for externally assigned data, such matrices may no longer have this property. 



--------------------------------------------------------------------------------

 Function: Determine whether the point is within the polygon, parameters: p refers to the target point, ptPolygon refers to the set of polygon points, and nCount refers to the number of sides of the polygon 

 Point_pos current_robot_pos (0.0, 0.0); is a structure with two data X and Y; 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574659287
  ```  


--------------------------------------------------------------------------------

We want to represent the point of each point cloud as a column chart with a height of Z, so as to draw a three-dimensional column chart of the terrain. The effect and code are as follows. There is still room for improvement in the x effect, but it is basically formed 

 ![avatar]( d47d7472afd145998f1a16ddaedea802.png) 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574635786
  ```  


--------------------------------------------------------------------------------

We need to connect a straight line in the trajectory to represent the loop, and we need to draw a straight line connecting two point clouds 

 As shown below 

 ![avatar]( 8b28d980430f4aceac4a5eab59c9d97a.png) 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957461430
  ```  


--------------------------------------------------------------------------------

 rospy.exceptions.ROSSerializationException: field data[] must be float type   

 The type of array sent is a two-dimensional array, so this problem will occur. Change the array to a one-dimensional array, and this problem will not occur. 

 That is, just put the array xxx.flatten (). 



--------------------------------------------------------------------------------

 Farthest Point Sampling is a very common sampling algorithm, which is widely used because it can ensure uniform sampling of samples. 

 The summary is to iteratively select the farthest point from the existing set of sampling points. 

 FPS algorithm principle: 

 The code implementation is as follows: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574634091
  ```  


--------------------------------------------------------------------------------

Project a 3D point to a 2D image, find the edge of the image, and then reverse map to find the corresponding edge point

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957464068
  ```  


--------------------------------------------------------------------------------

Here the selection of a single point to display the point cloud is achieved,

Press and hold shift and add the left button to select a single point. After closing the display interface, the serial number of the selected point will be displayed.

 ![avatar]( ccc00486bb9741db80f77a07bc4e493e.png) 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957469791
  ```  


--------------------------------------------------------------------------------

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


--------------------------------------------------------------------------------

 A simple image labeling tool, using the tkinter production interface, open the folder where the picture is located to start labeling the picture. All the code can be contained in only one file, and there is no need to install complex dependencies. The effect is as follows:  

 ![avatar]( fecc9226fe894b6697d09f5378bf3e16.jpeg) 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574668039
  ```  


--------------------------------------------------------------------------------

The code implements the volume measurement of the volume target in the Kinect V2 + PCL.

 ![avatar]( 6aac6fd4d1714e93900907b5a8d4f4c7.gif) 

Process:

1. Capture point clouds

2. Space clipping

3. Downsampling

4. Filtering

5. Plane division to find the ground

6. Plane segmentation to find the target top surface

7. Calculate area, height and volume 

 ![avatar]( 6445f9aac9c04c1695637f385ca16e66.png) 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 202402030957464911
  ```  


--------------------------------------------------------------------------------

Now the calibration procedures for lidar and cameras are basically under the Ubuntu framework, and they are all C++ code. The dependencies that need to be installed are also more complicated, so I wrote a python version of the calibration program. The dependencies are very simple, and the Windows system can also run. And the code is simple. A file is done, in line with the simple and easy style of python. 

 First, the renderings after the final calibration: 

 ![avatar]( a0bcc54a55bd49a6d58e3ecbf6d0a5dc.png) 

 ![avatar]( a3f2bbbbe3d0c8bacc42b43f9dbc97a5.png) 

 The idea of calibration is relatively simple: 

 Manually select N calibration points on the image 

 2 Manually select N calibration points on the point cloud (each point corresponds to a point on the image, and the order should also be the same) 

 3. Calculate the rotation projection matrix of the two by the PNP method, that is, the external parameter matrix 

 Schematic diagram of the first step: 

 ![avatar]( 80aedde1ff6050a98e003998fa4f6a0d.jpeg) 

 Schematic diagram of the second step: 

 ![avatar]( 548297637990f5f5d1217f54dcc9fd98.jpeg) 

 Finally, add the code: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574631166
  ```  
 The DJI radar I'm using here has more dense points, making it easier to calibrate using my method. Rotating 16- and 32-line radars can also be calibrated using this method, but the calibration points will be relatively difficult to select. 



--------------------------------------------------------------------------------

(With open3d python code) The idea is very simple, that is, to project the point coordinates of each three-dimensional onto the image coordinates, pay attention to the points: 

 1. When projecting, there is a resolution parameter, that is, a point is projected every few meters 

 2. The coordinates should not overflow the coordinate range of the image. 

 The effect is as follows: 

 ![avatar]( 4948d41841f84c058eb88c561346182a.png) 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574625517
  ```  


--------------------------------------------------------------------------------

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


--------------------------------------------------------------------------------

The code comes from livox_mapping, let me briefly say the conclusion: 

 Outlier extraction: the distance from the left and right points is greater than one-tenth of the depth value 

 Plane point extraction: mainly calculated by the curvature of the four points on the left or right less than 0.001; 

 Corner extraction: there are several main sources 

 Flat corner points, both left and right are flat and the angle between the planes is 60-120; (can be understood as the edge feature points of square columns) 

 Breakpoint corner: (can be understood as the scanning point from the edge of the object to the distance) According to the distance between the current point and the left and right nearby points, the breakpoint threshold is 0.1; and the point on one side is a plane; the distance between the point and the point is not too far; the distance between the farthest point does not exceed one-twentieth of the depth value; the plane synthesized by the current point and the farthest point, and the angle between the current point vector, the angle is 37 degrees to 143 degrees; 

 Other livox project feature extraction is similar, understand this basic other are similar; 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574616749
  ```  


--------------------------------------------------------------------------------

Sometimes we want to intercept point clouds from a tricky angle,

Or you want to capture a point cloud in a polygonal region.

It may not be so convenient to intercept with code,

At this time, visual cropping is more convenient and simple. 

 ![avatar]( 14d6e53b4daa423b82b5efc9a18181c4.png) 

 The code is as follows: 

  ```python  
After clicking on the GitHub Sponsor button above, you will obtain access permissions to my private code repository ( https://github.com/slowlon/my_code_bar ) to view this blog code. By searching the code number of this blog, you can find the code you need, code number is: 2024020309574668275
  ```  


--------------------------------------------------------------------------------

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


--------------------------------------------------------------------------------

I tried it with the dataset shared by others. The indoor mapping problem is not big, and the outdoor is still uncertain. 

 ![avatar]( 76f8e68c61e34470a075d99aa5649080.jpeg) 

 ![avatar]( 2081b5910eed49549baeb85214835599.jpeg) 

 ![avatar]( 9b60d40b072f4961b4f58c4054361a19.jpeg) 

 ![avatar]( 618834e687b14f4bb666efedf34fded3.jpeg) 

 ![avatar]( c850acaf482448a692b8fd7b76deee90.jpeg) 



--------------------------------------------------------------------------------

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



--------------------------------------------------------------------------------

