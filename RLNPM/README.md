# Ball Detection, Pose and Velocity Detection

The ball is detected through the rgbd camera and Depth and Color streams are generated. 
the raw generated data are converted to the numpy arrays and they are shown as follows through the opencv library:

Inline-style: 
![alt text](Camera/Color_Image.png "Raw Color RGB Image")

Inline-style: 
![alt text](https://github.com/Afshin1997/Afshin1997.github.io/blob/main/RLNPM/Camera/Depth_Image.png "Raw Depth Image")

Inline-style: 
![alt text](https://github.com/Afshin1997/Afshin1997.github.io/blob/main/RLNPM/Camera/Blurred_Image.png "Blurred Image")

Inline-style: 
![alt text](https://github.com/Afshin1997/Afshin1997.github.io/blob/main/RLNPM/Camera/hsv_Image.png "HSV Image")

Inline-style: 
![alt text](https://github.com/Afshin1997/Afshin1997.github.io/blob/main/RLNPM/Camera/mask_yellow_Image.png "Mask Yellow Image")

Inline-style: 
![alt text](https://github.com/Afshin1997/Afshin1997.github.io/blob/main/RLNPM/Camera/Disparity_Image.png "Disparity Image")

Inline-style: 
![alt text](https://github.com/Afshin1997/Afshin1997.github.io/blob/main/RLNPM/Camera/Spatial_Filtered_Image.png "Spatial Filtered Image")

Inline-style: 
![alt text](https://github.com/Afshin1997/Afshin1997.github.io/blob/main/RLNPM/Camera/Temporal_Filtered_Image.png "Temporal Filtered Image")

Inline-style: 
![alt text](https://github.com/Afshin1997/Afshin1997.github.io/blob/main/RLNPM/Camera/Depth_Filtered_Image.png "Depth Filtered Image")

Inline-style: 
![alt text](https://github.com/Afshin1997/Afshin1997.github.io/blob/main/RLNPM/Camera/Hole_Filled_Image.png "Hole Filled Image")
