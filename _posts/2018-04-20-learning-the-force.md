---
layout: post #always use this
title: Learning the force: Estimating End-Effector force in Robots #This becomes the title of the page
date: 2018-04-20
categories: [compliant robotics, force estimation]
---
Force sensors, though gradually becoming cheaper, are still expensive tools. Various companies are trying to alleviate these expenses by offering estimation of the end-effector forces using the supplied motor currents [^1]. These techniques are usually applied to lightweight robots that are made for human-machine interactions. Outlining the method of how one can go from motor currents to end-effector force estimation in a way that can be applied to any robot would be of interest to both industry and researchers as it is a low-cost gateway drug to more advanced compliant control techniques.

The student will be working with ROS: robotic operating system. At its core it is a middleware solution that implements a set of standards for communication between process. It's been used by a variety of researchers and programmers around the world to control anything from industrial robots, to drones, to unmanned boats. There is a wealth of packages openly available, and work may already exist on force estimation based on motor currents that would be of interest to the student.

In the Department of Engineering Cybernetics, we have recently acquired a robot system containing two industrial KUKA KR16 robots. With a maximum payload of 16 kg at the end-effector, these are heavy duty machines. They are controlled using two KRC2 robot controllers which we communicate to with ROS. The KUKA Robot Sensor Interface (RSI) that connects our computer and the KRC2s allows us to read both the force/torque (FT) at the end effector using our FT-sensor, and to read the supplied currents to the motors [^2].  Figuring out a mathematical model for how the motor current becomes the joint torques, and subsequently the torque at the end-effector is not a simple task. From motor to joint there may be gears and belts [^3] giving friction and backlash, making it difficult to model. From joint torques to end-effector FT we have to calculate the Jacobian from the forward kinematics. 

In this project the student will investigate whether the joint torques, and subsequentially the end-effector force can be estimated using modern novel learning and estimation techniques such as neural networks, transfer entropy [^4], etc. 

## Prerequisites ##

1. Interest in estimation and learning techniques
2. Experience with Ubuntu (Ideally ROS as well)
3. Experience with Python and C++

## Tasks ##
1. Investigate modern work in the field and whether ROS packages exist
2. Conduct experiments on both KR16 robots and UR robots for data gathering
3. Evaluate estimation techniques

## Further work ##
When considering force-estimation for control scenarios, a limiting factor is the calculation time of the estimation technique. Ideally the end-product from this would be a ROS node that listens to the motor current messages from the KUKA robots and sends out an estimate of the force and torque at the end-effector, and the joint torques. If the estimated forces are to be used in feedback control, the estimation must run at the timescale of milliseconds. This is a difficult task, so considering the runtime of estimation techniques must be performed early on. 

It would also benefit the community if the overall approach is systematized. This means to create a set of sufficient experiments for gathering the data irrespective of the number of joints and type of joints in the robot. Then to create a program that, given the robot description (URDF file) and the data, will generate the required estimater. Be it automatically train a neural network on the data or perform principal component analysis.

## Contacts ##

1. Tommy Gravdahl - Main supervisor
2. Mathias Hauan Arbo - PhD at the department (Co-supervisor)


## Links ##
[^1]: [https://www.kukakore.com/wp-content/uploads/2012/07/KUKA_LBR4plus_ENLISCH.pdf]
[^2]: Ivar Eriksen's Master Thesis
[^3]: [https://www.youtube.com/watch?v=iRKDfknqtbc]
[^4]: [https://ieeexplore.ieee.org/document/7487127/]
