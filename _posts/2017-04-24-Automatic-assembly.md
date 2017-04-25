---
layout: post #always use this
title: Automatic assembly  #This becomes the title of the page
date: 2017-04-21
categories: [nonlinear control, sliding mode]
---
# Automatic Assembly

## Introduction ##
Industrial robots, when calibrated correctly are precise machines capable of performing the same tasks again and again. In free moving motions, this is true, but when the robot is to assemble something with part tolerances lower than the angular precision of the robot, or with uncertainty in gripping/positioning, this is not the case. When interaction can occur, the control process becomes an entirely different beast, and a variety of methods exist to handle this. Some consider a finite state machine, basically switching between different controllers as the task progresses e.g. 
 - 1. position control to move to object,
 - 2. force threshold to know when you touch the object,
 - 3. active compliance to push the object into its hole 
some try to handle this with mechanical compliance e.g. the SCARA robot which is mechanically compliant in the horizontal plane, and others try to create more general analytical controllers.

## Project ##
In this particular project, we are looking at an assembly process that is to be performed for a partner company of SINTEF with supervision both from SINTEF and Mathias Hauan Arbo, a PhD candidate working on advanced robotic assembly. The project will let you work 
 - hands-on with large industrial robots,
 - both with the industry and academia.

The objects to be assembled is being discussed at the moment, and will be ready for when the project begins. 
