# Panoptic3D Dataset

### A multi-view, multi-modal dataset for mobile 3D perception compatible with nuScenes

<img src="assets/detection_low_quality.gif" alt="3D_det"/>

Multi-view 3D perception is a fundamental task for autonomous systems. However, existing datasets like nuScenes are limited to driving scenes. Its a personal research project to create a multi-view, multi-modal dataset for mobile 3D perception, which includes various urban environments in Seoul, Korea and LA, USA, where humans or robots can move around, such as campuses, city steets, crosswalks, etc. 

<!-- <div style="text-align: center;">
  <img src="assets/Sensor_configuration.svg" alt="dataset_creation_process" width="400"/>
</div> -->
<img src="assets/Sensor_configuration.svg" alt="dataset_creation_process" width="500"/> [Detailed dataset creation process](Dataset_creation.md)

### Features:
- Data types
  - Multi-view perspective images, 360-degree images, LiDAR point clouds, IMU data, camera parameters
- Annotation types
  - Camera poses, 3D bounding boxes (work in progress)
- nuScenes compatibility
  - Exacly same structure as nuScenes dataset (relational database)
  - Compatible with nuScenes devkit APIs

### Scenes:
| Location | Trajectory | Sample 360-degree image |
| --- | --- | --- |
| USC Campus, LA | <img src="assets/trajectory_la_campus.png" width="150"/> | <img src="assets/vis_la_campus_sample1.png" width="250"/> |
| USC Campus town, LA | <img src="assets/trajectory_la_campus_town.png" width="150"/> | <img src="assets/vis_la_campus_town_sample1.png" width="250"/> |
| Changcheon-dong, Seoul | <img src="assets/trajectory_changchundong.png" width="150"/> | <img src="assets/vis_changchundong_sample1.png" width="250"/> |
| Sinchon-dong (daytime), Seoul | <img src="assets/trajectory_sinchon_daytime.png" width="150"/> | <img src="assets/vis_sinchon_daytime_seq1.png" width="250"/> |
| Sinchon-dong (night), Seoul | <img src="assets/trajectory_sinchon_night.png" width="150"/> | <img src="assets/vis_sinchon_night_sample1.png" width="250"/> |
