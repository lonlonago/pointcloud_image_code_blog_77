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

