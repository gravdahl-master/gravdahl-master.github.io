---
layout: post #always use this
title: Design of extentded ride control system for SES    #This becomes the title of the page
date: 2017-04-21
categories: [nonlinear control, sliding mode]
---
# Design of extentded ride control system for SES #

A surface effect ship (SES) is a marine vehicle with a catamaran type hull and flexible rubber seals in the bow and stern end to enclose an air cushion that have high speed and superior sea keeping performance in high sea states compared to conventional catamarans [1]. SES is equipped with a lift system consisting of lift fans, and Vent Valves (VV) where the set of lift fans blow air into the air cushion with constant speed to pressurize it where the opening of the VV are controlled to generate desired lift which can carry close to 80% of the ships mass during transit. 

Umoe Mandal is currently the only shipyard in the world that launches SES. The shipyard has delivered several SES to the Norwegian Navy, such as the MTB Skjold class and the Mine Countermeasure Vessels (MCMV) series. Recently, the yard has focused on providing SES (WAVECRAFT) to the offshore wind industry.

In the recent years, different aspects of SES have been investigated. As a result, several new dynamic models and control systems have emerged from the research community. This include isolated or individual systems for heave & pitch control, sway control, and roll damping. However, there is a lack of comprehensive model which includes all (or nearly all) degrees of freedom related to ride control system. 

The proposed thesis includes the following tasks:
### Modeling: ### This task needs incorporating and combining the existing sub-models to create a single 4 DOF model (sway, heave, roll, and pitch) that defines the maneuvering behavior of SES in low speed operations. Both process plant model for simulation purposes and a control plant model for control system design and stability analysis should be developed.
### Control: ### this task unfolds in two parts. The first part includes further development of existing components of ride control systems such as (sway control, heave control, heave & pitch control, roll control). The second part is to design a switching (supervisory) hybrid controller that could automatically decide and prioritize which DoFs should be regulated with higher priority based on the current environmental conditions. Then, the supervisor should select the appropriate controller from the bank of the controllers developed in the former part and place the selected controller in the feedback loop.

Programing skills with Matlab and Simulink are required. The project may involve model testing at laboratories in SINTEF Ocean. The work will be supervised by 

Professor Jan Tommy Gravdahl from Department of Engineering Cybernetics, Adj. Associate professor Vahid Hassani from Department of Marine Technology, and Dr. Øyvind Auestad from Umoe Mandal. 

[1] Øyvind F. Auestad, (2015). The Boarding Control System. Ph.D. thesis, Norwegian University of Science and Technology
