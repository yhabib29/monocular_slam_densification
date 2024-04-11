# Monocular SLAM Densification

This repo provides qualitative results illustrating our work on Monocular SLAM Densification. 
In this example, we build on ORB-SLAM 3 which provides precise camera pose estimation and triangulate sparse depth with metric scale. 
For the densification, we leverage ZeroDepth model to predict a dense depth map for every keyframe. 
We assume that this DNN predicts depth up to a global factor, and use the SLAM outputs to correct the scale. 
Lastly, we integrate Voxblox to build a voxel map iteratively from the resulting scaled dense depth maps and their corresponding estimated camera pose. Further details are provided in the publishes papers.

[Link to the Github Page](https://yhabib29.github.io/monocular_slam_densification/)

## Publications

1. Y. Habib, P. Papadakis, C. Le Barz, et al., « Densifying slam for uav navigation by fusion of monocular depth prediction », in 2023 9th International Conference on Automation, Robotics and Applications (ICARA), 2023, pp. 225–229. doi: [10.1109/ICARA56516.2023.10125712](https://doi.org/10.1109/ICARA56516.2023.10125712)

2. Y. Habib, P. Papadakis, A. Fagette, et al., « From sparse SLAM to dense mapping for UAV autonomous navigation », in Geospatial Informatics XIII, K. Palaniappan, G. Seetharaman, and J. D. Harguess, Eds., International Society for Optics and Photonics, vol. 12525, SPIE, 2023, p. 125250C. doi: [10.1117/12.2663706](https://doi.org/10.1117/12.2663706)

3. Y. Habib, P. Papadakis, C. Le Barz, et al., « Monocular SLAM densification for 3D mapping and autonomous drone navigation », Ecole nationale supérieure Mines-Télécom Atlantique, Thesis, Mar. 2024. [Online]. Available: https://theses.hal.science/tel-04521284

4. Y. Habib, P. Papadakis, C. Buche, et al., Dense, metric and real-time 3d reconstruction for autonomous drone navigation, Journées des Jeunes Chercheurs en Robotique (JJCR 2021), Poster, Oct. 2021. [Online]. Available: https://hal.science/hal-04184995
