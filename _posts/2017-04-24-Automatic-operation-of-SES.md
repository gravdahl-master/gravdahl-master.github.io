---
layout: post #always use this
title: Automatic operation of Surface Effect Ship (SES)    #This becomes the title of the page
date: 2017-04-21
categories: [nonlinear control, sliding mode]
---
# Automatic operation of Surface Effect Ship (SES) #

A surface effect ship (SES) is a marine vehicle with a catamaran type hull and flexible rubber seals in the bow and stern end to enclose an air cushion that have high speed and superior sea keeping performance in high sea states compared to conventional catamarans [1]. SES is equipped with a lift system consisting of lift fans, and Vent Valves (VV) where the set of lift fans blow air into the air cushion with constant speed to pressurize it where the opening of the VV are controlled to generate desired lift which can carry close to 80% of the ships mass during transit. 

Umoe Mandal is currently the only shipyard in the world that launches SES. The shipyard has delivered several SES to the Norwegian Navy, such as the MTB Skjold class and the Mine Countermeasure Vessels (MCMV) series. Recently, the yard has focused on providing SES (WAVECRAFT) to the offshore wind industry.

Due to complex nature of SES, day-to-day operation of SES involves continuous manual adaptation of large number of tuning parameters. The followings are among the most important settings and parameters that needs regular adaptation:
* A SES is very trim sensitive, so the operator must often transfer fuel from various fuel tanks or adjust the seawater level in ballast tanks. The trim adjustment could be automated since a desired trim angle, for various conditions, is known in advance.
* The operator must manually set certain control system parameters for the ventilation valve system (air out of the air cushion) as well as adjusting the lift fan engine revolutions (air into the air cushion). This could be automated or semi-automated such the operator could choose from a set of predefined settings, namely "eco-mode", "speed" or "comfort".
* The operator must specify the extra air pressure that is in the stern bag, relative to the air cushion. This procedure could be automated as function of the air cushion pressure and the environmental conditions.

The proposed thesis includes modeling and developing control algorithms that could automate the above-mentioned aspects of SES operation. Currently simple, but effective, SES models exists, but these needs to be further developed and verified. 
Programing skills with Matlab and Simulink are required. The project may involve model testing at laboratories in SINTEF Ocean. 

The work will be supervised by 

Professor Jan Tommy Gravdahl from Department of Engineering Cybernetics 
Adj. Associate professor Vahid Hassani from Department of Marine Technology, 
and Dr. Øyvind Auestad from Umoe Mandal.

[1] Øyvind F. Auestad, (2015). The Boarding Control System. Ph.D. thesis, Norwegian University of Science and Technology.
