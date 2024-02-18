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

