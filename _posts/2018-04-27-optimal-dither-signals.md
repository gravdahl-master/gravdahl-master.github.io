---
layout: post #always use this
title: Optimal dither signals for improved resolution and accuracy in digital-analog converters used for closed-loop control
date: 2018-04-27
categories: [nonlinear control, sliding mode]
---

Physical implementations of digital-to-analog converters (DACs) introduce various non-ideal effects, including element mismatch, thermal and semiconductor noise, slew-rate limitations, and glitches caused by non-ideal transistor switching. These effects come in addition to the fundamental error sources of aliasing and quantization that occur in a digital signal processing system, due to discretization in both in time and value.

![DAC prototype]({{site.baseurl}}/assets/prototype_dac.jpg "DAC prototype")

**When applying a DAC for high precision motion control, DAC-errors deteriorate the achieved performance.** Hence, it is of interest to mitigate them. Aliasing is reduced by reconstruction filtering and interpolation, and quantization error is eliminated using small-scale noise dithering. Element mismatch can be compensated for using several methods, such as dynamic element matching or physical calibration, and slewing can be partially reduced reduced by oversampling.

**One method that has not been studied in detail yet is large-scale dithering, which can mitigate element mismatch, as well as glitches, and possibly other effects.** Work is needed to find ways to maximize the effect of such dither signals, and to study the what happens when dither is applied to closed-loop systems.

![Effects of applied dither]({{site.baseurl}}/assets/dither_effects.png "Effects of applied dither")

* Learn how to use a common high-speed instrumentation digital-analog converter (use LabVIEW (simple) or VHDL/Verilog (hard) to interface with the device and to enable closed loop control of a system).
* Study models of non-linear and non-ideal effects in digital-analog converters.
* Determine how well the models fit with actual digital-analog converter behavior (model validation).
* Study how different dither signals impact the distortion in digital-analog converters; that is determine the model properties.
* How does the introduction of feedback control impact the effect of the dither signals in closed-loop?
* Use optimization techniques to find optimal dither signals that minimize distortion and error (possibly apply input shaping methods to generate optimal dither signals).

