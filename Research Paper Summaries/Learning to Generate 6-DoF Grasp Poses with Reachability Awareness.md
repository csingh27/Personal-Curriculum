**Learning to Generate 6-DoF Grasp Poses with Reachability Awareness**  

**TASK DEFINITION**  
* Given : Unstructured environment with unknown objects   
* Given : Unrestricted workspace with reachability awareness  
* Decide which sampled grasp pose candidates are more reachable  
* Grasp as many objects as possible from dense clutter with minimal efforts  

**ASSUMPTION**  


**MAIN IDEAS**  
* Voxel-based 3D CNN to generate 6DOF Grasp poses  
* Simultaneously learns grasp reachability  

**PIPELINE(SIMPLIFIED)**  
* Point cloud  
* Object point cloud obtained from planar segmentation of point cloud  
* Grasp pose sampling to obtain grasp poses  
* Voxelization of point cloud for each grasp pose and transformed w.r.t. grasp pose so that the robot hand is aligned and fixed to the top grasping position  
* 3D CNN estimates the grasping stability score of each grasp pose  
* Reachability predictor estimates reachability score for each grasp pose  
* grasping score is obtained by multiplying reachability score and stability score  
* Pose with the highest score is selected  
 
**Special features**  
* Trained on large scale synthetic dataset  
* Domain-invariant  
* 82.5 % Success Rate on novel objects  

**FURTHER REVIEW**  
* 

**LIMITATIONS**  
* 
