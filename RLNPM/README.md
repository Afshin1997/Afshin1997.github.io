# Ball Detection, Pose and Velocity Detection

The ball is detected through the RGBD camera, and depth and color streams are generated. The raw generated data are converted to numpy arrays and are shown as follows through the OpenCV library:

<table>
  <tr>
    <td><img src="Camera/Color_Image.png" alt="Raw Color Image" style="width: 100%;"/></td>
    <td><img src="Camera/Depth_Image.png" alt="Raw Depth Image" style="width: 100%;"/></td>
  </tr>
</table>

The following processes are performed on the RGB image:

<table>
  <tr>
    <td><img src="Camera/Blurred_Image.png" alt="Blurred Image" style="width: 100%;"/></td>
    <td><img src="Camera/hsv_Image.png" alt="HSV Image" style="width: 100%;"/></td>
    <td><img src="Camera/mask_yellow_Image.png" alt="Mask Yellow Image" style="width: 100%;"/></td>
  </tr>
</table>

The following filters are applied to the depth images to obtain noiseless information about the position of the ball in 3D environments.

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

The positions can be detected correctly in millimeters ($mm$) in 3D.

Thereafter, a Kalman filter is applied to estimate the position of the ball when there is no information from the camera that could be fed into the network. During these periods, the data from the Kalman filter will be fed to the network, and once some data are derived from the camera, the Kalman filter will be updated.
