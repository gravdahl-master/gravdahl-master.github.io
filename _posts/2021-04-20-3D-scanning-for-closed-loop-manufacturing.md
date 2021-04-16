---
layout: post
title: 3D-scanning for closed loop (additive) manufacturing
date: 2021-04-20
categories: [Computer vision, Robotics]
---

3D printing, as we know it today, is a relatively new technique for production of parts by adding more and more material on-top of a buildplate. Material ranging from a wide range of plastics to a wide range of metals. Most commercial plastic 3D printers build in "open-loop" and just follows instructions on where to move, how fast to move and how much material to extrude at a given time. If something were to go wrong, or the printing conditions were to change considerably, the printer would not notice and would happily keep printing, possibly making a mess instead of the intended product. It is therefore of interest to explore the use of different sensors and 3D-scanning techniques for monitoring and error correction in 3D printing. Down the road, this may led to more autonomous and robust additive manufacturing systems.

In this specialization project, you will get the chance to delve into 3D printing, in addition to writing a ROS package for a laser line sensor, 3D depth camera, or similar sensor, that will later be used in research on 3D printing and closed-loop 3D printing. The ROS package should also be general enough that it can be used in other application, for instance robotized welding.

## Prerequisites ##

1. TTK4255 Robotsyn or similar experience
2. Experience with Ubuntu and git
3. Experience with Python or C++
4. Experience or interest in learning ROS

## Tasks ##

1. Familiarize yourself with laser and camera sensors for capturing geometric information
2. Write a ROS package for a laser scanner or other sensor
3. Experiment/capture data with the sensor on a 3D printer system

## Further work ##

Depending on how far the project gets, experiment with estimating the height and width of 3D printer tracks could be one option. This is up to your ambition. The end goal is to try and measure the error between the physical 3D print and the CAD model.

## Contacts ##
1. Andreas Hanssen Moltumyr - Project Lead
2. Jan Tommy Gravdahl - Main supervisor

![Franka_AM_Setup](../assets/extruder_mounted_to_franka.jpg)
Fig. 1: Franka Emika Panda robot with a custom built FDM extruder.

![Laser_Line_Scanner](https://www.wenglor.com/fileadmin/_processed_/4/c/csm_B_PRO_MLSL_1818ec2c70.jpg)
![Oak-D](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTqOjZD4dzxM0PANytdisiOuFvTLZndQS6_yQ&usqp=CAU)

Fig. 2: Laser line scanner and Oak-D stereo camera.