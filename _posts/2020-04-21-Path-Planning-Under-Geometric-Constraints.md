---
layout: post #always use this
title: Path Planning Under Geometric Constraints #This becomes the title of the page
date: 2020-04-21
categories: [nonlinear control, path planning]
---

When placing a cup on a table, the minimal description of what we are trying to achieve can be described by the geometric constraints involved. We want to keep the normal vector from the table and the axis of the cup to be parallel, and we want to make the bottom plane of the cup and the table coincident. For those who have used CAD software, this is how you often place parts in the model. If a robot would be able to do this in a simple way, we would be able to exploit the symmetry of the cup to place it anywhere that is available on the table. This minimal description would simplify robot programming, allowing for more succinct task descriptions. One of the problems with this succinct task description is figuring out a feasible path from wherever the cup is now to the end-goal (table-bottom coincidence). This project aims to investigate planning in the motion subspace described by geometric constraints to achieve various tasks. Similar work includes [^1], where you sample a null-space of geometric constraints to figure out a path to a goal state. For those who are familiar with path-planning, this project will potentially involve rapidly-exploring random trees and CAD models. The end-goal of this project is to be able to execute the results on a robot.

In the specialization project, part of the work will include evaluating how you want to represent the geometric constraints. Perhaps you like transformation matrices, or you prefer quaternions, or perhaps you'd like to try the more appropriate conformal geometric algebra. This is a point of discussion that will be evaluated in the specialization project.
    
## Prerequisites ##

1. Experience with ROS and interest in CAD
2. Experience with Ubuntu and git
3. Experience with Python or C++

## Tasks ##

1. Familiarize yourself with geometric constraints
2. Investigate path planning in a chosen representation
3. Find a path for a simple task

## Further work ##

Depending on how far the project gets, experiments will either be performed with a set of simple objects, or a full-scale CAD-based assembly will be performed. This is up to your ambition. The end goal is to create a representative experiment and trying it out in the robot lab with one of the available robots.

## Contacts ##

1. Mathias Hauan Arbo - Project lead
2. Tommy Gravdahl - Main supervisor

[^1]: [Nikhil Somani's PhD, Chapter 5: Motion Planning](https://mediatum.ub.tum.de/doc/1431736/1431736.pdf)
