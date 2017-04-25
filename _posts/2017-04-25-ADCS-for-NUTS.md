---
layout: post #always use this
title: 3D printing by robot   #This becomes the title of the page
date: 2017-04-25
categories: [nonlinear control, sliding mode]
---
# NTNU Test Satellite – NUTS: #

As a part of the national student satellite program, the NUTS CubeSat project was initiated at NTNU in 2010. 
The projects goal is to give hands-on experience to students within different fields of satellite technology. 
This includes planning, specification, design, construction, launch and operation of a satellite.
The construction of a satellite is a multi-disciplinary field. To succeed, the project needs highly 
motivated and interested students with a different backgrounds. This technical complex project will 
serve as a challenge for all persons involved.
 
The main parts of the satellite bus are:
 
* Power system (solar cells and batteries)
* Attitude and orbit control
* Mechanical system (structures and mechanisms)
* TT&C (telemetry, tracking and command)
* Thermal system
* On-board data handling/On Board Computer (OBC)
* Payload and experiment
 
All project members will be assigned their individual problem description. 
This final assignment text will be created together with the student, to fit both the project's needs and the student's fields of interest.
 
As we are a multidisciplinary group with project members from several departments, 
different types of team- and group work must be expected. It will be required that the student joins 
weekly meetings with the rest of the team (consisting of staff, other project/master students and other students) 
to share experience and knowledge.

### ADCS – Attitude Determintation and Control System: ###
The assigment ccan consist of one or several of the follwing tasks:

* Calibration (av sensorer, vi har bias i sensorene, magnetometer, gyro, solsensor, earth sensor)
* Test
  * Magnetometer støy – hvordan oppfører de seg i forskjellige omgivelser, Helmholtz coil test,
  * Gyro test, få data på forskjellige attituder
* Simulation of dynamics and control of NUTS (MATLAB - easiest)
  * Simulate orbit of satellite with appropriate perturbation model (J2 effects, albedo radiation, lunar gravity influences, solar   radiation pressure, atmospheric drag etc.)
  * Develop a model for estimator (EKF vs. EQUEST vs. other nonlinear estimators)
  * Determine behaviour of satellite based on appropriate control law. Attitude stabilization.
  * Determine how satellite behaves with attitude control by use of sun sensor, magnetometer, gyro independently
* Hybrid Kalman Filter (continuous and discrete) for NUTS
* If using Kalman Filter: Analysis of selecting weights for process noise covariance matrix Q and sensor noise covariance R.
* Research on Unscented Kalman filter for estimating attitude of satellite.
* Analysis of attitude control: damping control (detumbling) and use of PID (or PD) for three-axis stabilization control (magnetic coil). This may include simulation of a satellite in a virtual environment with timeframe: separation-to-orbit insertion as well as perturbation simulations on how the satellite would behave while in orbit.

