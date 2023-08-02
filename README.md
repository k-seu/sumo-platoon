# sumo-platoon
![输入图片描述](README_md_files/fa6af760-3121-11ee-92b0-8b71f5e918f9.jpeg?v=1&type=image)
**Fig 1. Logic of platform**

As described in Fig 1, the platform mainly has 5 parts, the  system structure of the platform is following:

## 1.  Environment Part
    
###  - data convertion from existing dataset
    
###  - generate traffic directly from sumo
    
## 2. Communication Part
    
###  -V2V communication  (veins)
    
##  3.Perception Layer
    
###  -vehicle get information from surrounding environment (relative distance, velocity with other vehicles, road information...)
    
##  4.Planning & Decision Layer
    
###  -Route planning (depends on task, usually from a start point to an end point)
    
###  -Behavior planning (Behavior decision: lane change, car follow, stop, etc.)
    
###  -Motion Planning
    
####  trajectory generation
    
####  trajectory following
    

 -follow waypoints
    
 -directly follow trajectory (Stanley method)
    

##  5.Control Layer
    
###  -Controller (generate the input of the low-level dynamics(steering, throttle commands)
    
###  -Low-level dynamics
    
####  **PM (point mass)**
    

input: acceleration in x and y direction
output: position, velocity for the next time step

#### **Bicycle model**
  input: desired acceleration and steering commands
 output: position, velocity, steering angle for the next time step
 
