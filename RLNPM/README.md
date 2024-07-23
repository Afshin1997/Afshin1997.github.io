# Ball Detection, Pose and Velocity Detection

The ball is detected through the rgbd camera and Depth and Color streams are generated. 
the raw generated data are converted to the numpy arrays and they are shown as follows through the opencv library:

<table>
  <tr>
    <td><img src="Camera/Color_Image.png" alt="Raw Color Image" style="width: 100%;"/></td>
    <td><img src="Camera/Depth_Image.png" alt="Raw Depth Image" style="width: 100%;"/></td>
  </tr>
</table>


<table>
  <tr>
    <td><img src="Camera/Blurred_Image.png" alt="Blurred Image" style="width: 100%;"/></td>
    <td><img src="Camera/hsv_Image.png" alt="HSV Image" style="width: 100%;"/></td>
    <td><img src="Camera/mask_yellow_Image.png" alt="Mask Yellow Image" style="width: 100%;"/></td>
  </tr>
</table>


<table>
  <tr>
    <td><img src="Camera/Disparity_Image.png" alt="Disparity Image" style="width: 100%;"/></td>
    <td><img src="Camera/Spatial_Filtered_Image.png" alt="Spatial Filtered Image" style="width: 100%;"/></td>
    <td><img src="Camera/Temporal_Filtered_Image.png" alt="Temporal Filtered Image" style="width: 100%;"/></td>
  </tr>
  <tr>
    <td><img src="Camera/Depth_Filtered_Image.png" alt="Depth Filtered Image" style="width: 100%;"/></td>
    <td><img src="Camera/Hole_Filled_Image.png" alt="Hole Filled Image" style="width: 100%;"/></td>
  </tr>
</table>
