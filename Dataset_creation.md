### 1. Sensor Configuration
<img src="assets/sensor_hardware.png" width="300"/>

### 2. Sensor Calibration
#### (1) Virtual camera

<img src="assets/virtual_cameras.png" width="600"/>
To mitigate the inherent distortion of 360-degree images, we split the 360-degree image into six regions using perspective projection, treating each as a separate virtual camera.

#### (2) Intrinsic/Extrinsic calibration

<img src="assets/calibration.png" width/>

We first calibrated the sensor extrinsincs (sensor coordinate transformation matrices). Then, we calibrated each projected camera image’s intrinsics with the checkerboard method. An overview of the sensor coordinate systems is shown below: 

<div style="text-align: center;">
    <!-- <img src="assets/coordinate_system_transformation.png" width="450"/>
    <img src="assets/coordinate_system.png" width="450"/> -->
    <img src="assets/coordinate_system_transformation.png" width="450"/>
    <img src="assets/coordinate_system.png" width="450"/>
</div>

### 3. LiDAR-Camera Time Synchronization

<img src="assets/lidar_cam_sync.jpg" width="600"/>

### 4. LiDAR-IMU Odometry

<img src="assets/LiDAR-IMU odometry.gif" width="500"/>

We created accurate sensor movement trajectories (ego pose data) using LiDAR-IMU odometry using [Point-LIO](https://github.com/hku-mars/Point-LIO). 

### 5. 3D Bounding Box Annotation (in progress)

We've generated 3D bounding box annotations for objects in the scene using the [xtreme1](https://github.com/xtreme1-io/xtreme1). Since manual annotation is time-consuming, we are working on a automatic annotation to speed up the process.

### 6. Dataset Structuring (nuScenes format)

The dataset is structured in the same way as the nuScenes dataset using [this script](./nusc_dataset_gen.ipynb), allowing for easy implementation and evaluation with well-established open-source frameworks for 3D perception like nuScenes devkit APIs and MMDetection3D.