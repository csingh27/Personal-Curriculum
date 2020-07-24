**Dex-Net AR: Distributed Deep Grasp Planning Using a Commodity Cellphone and Augmented Reality App**  

**TASK DEFINITION**  


**ASSUMPTION**  


**PIPELINE (SIMPLIFIED)**  
* Record RGB images from iPhone  
* Extract noisy point cloud using Apple AR Kit (Based on Structure from Motion and SIFT)  
* Clean the point cloud  
* Transform into depth map using PyRender  
* use DexNet to find grasps  

**Special features**  

**FURTHER REVIEW**  
* 

**LIMITATIONS**  
* AR Kit fails to capture point clouds from featureless objects  
