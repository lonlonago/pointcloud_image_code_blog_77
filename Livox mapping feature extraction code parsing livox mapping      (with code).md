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
