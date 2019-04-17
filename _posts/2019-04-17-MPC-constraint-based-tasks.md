---
layout: post #always use this
title: MPC and Constraint-Based Task Specifications #This becomes the title of the page
date: 2019-04-17
categories: [nonlinear control, model predictive control]
---
When choosing what a robot is to do, the constraint-based task specification approach allows for fast and easy integration of multiple tasks. The specification allows tasks to be executed on any industrial robot for which the forward kinematics is known, and we can have easy sensor integration. Tasks are simple descriptions of some sort of error, say the distance between the end-effector and a point we want to track, and the convergence behavior we want for that task, e.g. converge to zero exponentially. A controller for constraint-based task specifications can take this information to figure out what the joint speed setpoints on the robot should be to achieve this. Since these controllers can be defined separately from the task specification, and they can be solved using nonlinear optimization, one can quickly imagine using a model predictive controller for the task. Examples of constraint-based task specification softwares include [eTaSL](https://rob-expressiongraphs.pages.mech.kuleuven.be/expressiongraph_doc/index.html) by Erwin Aertbelien, or [CASCLIK](https://github.com/mahaarbo/casclik) by Mathias Hauan Arbo. 

[CASCLIK](https://github.com/mahaarbo/casclik) started some investigation into the model predictive controller formulation for constraint-based task controllers, and this project will look at extending the work. Some of the major limitations of the current approach are:

1. the stability of the model predictive controller approach is not known,
2. the convexity of the optimization problem constraints is not known,
3. the current implementation is much too slow.

For more information on CASCLIK, check out the article[^1] or contact [Mathias](https://www.ntnu.edu/employees/mathias.arbo). 
This project will investigate and address these issues. The project will be in tandem with a project at the department of mechanical engineering that looks at the model predictive controller for robotic assembly. There will be possibilities of playing with a variety of simulated robots and tasks, doing everything and anything from simple collision avoidance to welding or assembling.  


## Prerequisites ##

1. Interest in model predictive control for robotics
2. Experience with Ubuntu and git
3. Experience with Python or C++


## Tasks ##

1. Familiarize yourself with model predictive control 
2. Investigate stability criteria 
3. Extend one of the two existing frameworks


## Further work ##

The project has the possibility of going in two main directions, experimental or theoretical. The theoretical road leads down to exploring the stability of the other controllers as well, commenting on the taxonomy of tasks that can be combined, figuring out how one can best design tasks such that the desired objectives can be achieved. The experimental road looks at extending one of the existing frameworks such that the model predictive controller can be applied in real-time robot control on one or some of the robot platforms available (KUKA KR16s, KUKA AGILUS, KUKA IIWA 4+, UR5, UR10, UR3, or potentially the franka emica). 


## Contacts ##

1. Mathias Hauan Arbo - Project lead
2. Tommy Gravdahl - Main supervisor

[^1]: [arXiv:1901.06713](https://export.arxiv.org/abs/1901.06713)
