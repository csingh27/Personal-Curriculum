**6-DOF Grasping for Target-Driven Object Manipulation in Clutter**  

**TASK DEFINITION**  
*Retrieve unknown target objects in structured clutter*  
*Grasp DOF : 6*  
*Workspace : Unconstrained*  
*Consider collisions : Yes*  
*Objects and environment : unknown*  

**ASSUMPTION**  
* Collisions between gripper (not arm) and scene  

**PIPELINE (SIMPLIFIED)**  
* Single View RGB-D Observation gives 3D Point Cloud  
* 3D Bounding box centred on target object  
* Cropped point cloud using Bounding box  
* using instance segmentation, point cloud just for the target object is obtained  
* Distribution of successful object-centric grasps is obtained by passing the target object point cloud and a latent vector through a VAE Decoder (Training in Simulation)  
* Grasps are scored based on collisions after passing it through a collision-graph  
NOTE : Collision checking is generally done in Simulation, but here instead it is generalized for unknown objects as collision-net is conditioned based on point-cloud observations  
 
**Special features**  
* Edge case : Removes blocking objects by means of collision-net prediction  
* Achieves a performance of 80.3 % in grasping novel objects in clutter on real robot despite being only trained in simulation  

**FURTHER REVIEW**  
* 

**LIMITATIONS**  
* Robot trajectory not considered in grasp generation  
* Open loop system  
