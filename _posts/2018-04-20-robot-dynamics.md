---
layout: post
title: Robot Dynamics with ROS and CasADi
date: 2018-04-20
categories: [industrial robotics]
---
ROS - the robotic operating system is a software suite with a large community. At its core it is a middleware solution that implements a set of standards for communication between process. It's been used by a variety of researchers and programmers around the world to control anything from industrial robots, to drones, to unmanned boats. ROS has a universal robot description format (URDF[^1]). This is an XML file that represents the robot model, it gives the position of reference frames, the types of joints in the model, and tags for describing the dynamics of the robot.

Robot control researchers are often interested in the kinematics and dynamics of the robot, but this information is often difficult to arrive at, or requires tedious work on paper. URDFs present an opportunity to generate the information automatically for any robot, given that the URDF is fully descriptive. This has already been achieved by the OROCOS[^2] and ROS community where the Kinematics and Dynamics Library (KDL)[^3] is _the_ go-to real-time kinematics and dynamics library. But for symbolic expressions, there's less available.

A library for using symbolic equations and doing algorithmic differentiation that is growing in popularity among robotics researchers is CasADi[^4]. It provides a framework to rapidly prototype optimization algorithms and symbolic equations that are close to production ready. By creating an open-source library to generate the symbolic equations from the URDF, you may simplify the life of researchers wanting to do model predictive control, path planning, timing optimization, and many other topics.

This project will be an extension of a library in development, and the forward kinematics have already been created. The student will be part of formulating the library structure and to participating in control experiments on both KUKA robots[^5] and UR robots.  

### Prerequisites ###
1. Interest in robot modeling and multibody dynamics
2. Experience with Ubuntu (Ideally with ROS as well)
3. Experience with Python (Potentially also C++)

### Tasks ###
1. Get familiarized with the URDF format and ROS
2. Get familiarized with CasADi
3. Create algorithms for generating symbolic expressions of dynamics parameters ($${M}(\vec{q})$$, $${C}(\vec{q},\dot{vec{q}})$$, $${G}(\vec{q})$$)
4. Evaluate the runtime of the equation and validity in simulations with Gazebo

### Further work ###
If time allows, we would like to see experiments on a UR5 to evaluate the accuracy of the models. Experiments to gather the data for estimating the inertia tags in the URDF would also be very helpful. In the Thrivaldi robotics lab [^5] we have a two KUKA robots equipped with a variety of objects affecting its inertial parameters. A final test of the parameter estimation would be run the procedure on this complicated scenario.

The software is initially aimed towards Python programmers and CasADi users, but many at the department use Matlab, and other symbolic expression libraries. Once the algorithms are created for Python, it should be easy to implement a Matlab version as well. Support for other symbolic expression libraries may prove difficult, but would be a welcomed extension of the project.

### Contacts ###
1. Tommy Gravdahl - Main supervisor
2. Mathias Hauan Arbo - PhD at the department (Co-supervisor)

[^1]:[ROS page on URDF](http://wiki.ros.org/urdf)
[^2]:[OROCOS homepage (outdated)](http://www.orocos.org/)
[^3]:[OROCOS - KDL (outdated)](http://www.orocos.org/kdl/UserManual/kinematic_solvers)
[^4]:[CasADi wiki](https://github.com/casadi/casadi/wiki)
[^5]:[Thrivaldi robotics lab](https://github.com/itk-thrivaldi)
