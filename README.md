# Machine Learning: Disaster Recovery Simulation
This project explores and applies machine learning concepts through a simulated search and rescue scenario. Python is used for the logic of a SAR bot inside of CoppeliaSim.

***Note: the .ttt file can only be opened in CoppeliaSim and contains the enirety of project.***

## Background
Real-time search-and-rescue robots are increasingly used to supplement the efforts of the first responders in areas affected by natural disasters. 
They are used to spot-check the situational awareness of people in distress, survey the extent of flood or tornado damage, evaluate the number of people that had not been evacuated from their neighborhoods, clean debris, and create passable routes.
### The Task
Create a virtual prototype of an autonomous robotic recovery system that demonstrates goal-seeking behaviors in navigating through a predefined area.

## The Simulation
### Simulation Environment
I created a rudimentary environment filled with debris, as it can depict a number of scenarios ranging from a collapsed building to a tornado stricken town.
Below is a screenshot from the simulation where we can see the boxed off environment, a number of cylinders and spheres, and our robot. 


The maroon cylinders represent static debris while the tan spheres represent loose debris. Each time the simulation is ran, the loose debris is thrown around the environment at random.
The red cylinder is our target and represents a person caught in the debris.


![simulation screenshot](https://github.com/Teeko98/machine-learning-disaster-recovery-simulation/blob/main/simulation-screenshot.png)

### Disaster Recovery
The robot moves forward and backward with the ability to rotate in either direction. It has a sensor that allows it to see a short distance in front of itself. 
The robot's logic is written in Python and instructs it to navigate the environment. It avoids colliding with debris detected by its sensor.
The robot creates an internal map as it explores the environment, preventing redundant searching of previously searched areas.
Once the robot detects the target, the simulation is complete.
