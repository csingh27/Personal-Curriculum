**Tactile Dexterity: Manipulation Primitives with Tactile Feedback**  

**TASK DEFINITION**  
*Manipulate an object from a known location to a desired location*  
*Manipulation primitives : Pushing, pulling, pivoting and regrasping*  

**ASSUMPTION**  

**PIPELINE (SIMPLIFIED)**  
* Contact state and object state are tracked  
* Contact state- Whether object is sticking or sliding relative to the robot palm  
* Object state- Targetting localized features of the object ,e.g. edges  
* Features extracted from contact state and object state can be used for tactile control  
* Contact state control- We regulate the applied forces on an object to enforce a desired contact state by monitoring the slip  
* Object state control- We track the pose of the object in real time and replan the trajectory to bring the object estimate to the goal  
* Sequences of primitives are used to achieve the task  
 
**Special features**  
* Manipulate an object from any pose to another on a table top while having reactive tactile behaviour (corrective action based on tactile feedback)  
* High resolution tactile sensors for accurate feedback  
* Reactive and robust to external perturbations  

**FURTHER REVIEW**  
* 

**LIMITATIONS**  
* Contact restrictions limited to simple mechanics and those that have interpretable tactile feedback  
* 
