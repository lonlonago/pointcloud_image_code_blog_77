 rospy.exceptions.ROSSerializationException: field data[] must be float type   

 The type of array sent is a two-dimensional array, so this problem will occur. Change the array to a one-dimensional array, and this problem will not occur. 

 That is, just put the array xxx.flatten (). 

