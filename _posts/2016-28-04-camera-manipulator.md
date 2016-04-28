---
layout: post #always use this
title: Robotic 3D imaging #This becomes the title of the page
date: 2016-04-19
categories: [robots]
---
# Robotic 3D imaging #

To inspect the quality of parts in a manufacturing process, consider using a 3D imaging device (stereo vision, 3D camera) attached to the end-effector of a robotic manipulator. The robotic manipulator will either move the camera over the object, or move the object in front of the camera to create a 3D representation of the object which can then be compared with a known CAD model of the object. The main objective is to design an algorithm planning the motion of the end-effector (with the camera), such that a high quality 3D representation of the object is achived.

1. Give a short introduction to 
  1. state-of-the-art 3D representations of objects and and their suitability for being used for quality inspection.
  2. methods for comparing 3D models with the objective of finding discrepency with respect to given design tolerances (e.g. length, diameter, straightness, etc) 
  3. robotic motion planning methods suitable for 3D imaging of objects.
2. Investigate the pros and cons of the following robotic set-ups for quality inspection: 1) The imaging device is placed on the robot arm, and the arm is moved around to give an as complete as possible representation of the (stationary) object. 2)The object is is moved around in front of a stationary imaging device to give an as complete as possible representation of the object. For instance, the former will be the obvious choice if the object is too heavy or too large to be lifted by a manipulator.
3. Consider having the 3D imaging device attached to the end-effector of a robotic manipulator. Design an algorithm planning the motion of end-effector of the manipulator based on a known CAD model of the object. The algorithm should be evaluated with respect to completeness of the achived 3D representation (coverage by the cameras field-of-view) quality of the achived 3D representation (estimated accuracy of the representation based on for instace the imaging quality and accuracy of end-effector positioning) and efficiency (time consumption of the total planned motion). Consider also the efficiency of the algorithm with respect to a new object and CAD model
4. Implement, test and verify the designed algorithm on a real robot manipulator.

Co-supervisor: Esten Grøtli, SINTEF
