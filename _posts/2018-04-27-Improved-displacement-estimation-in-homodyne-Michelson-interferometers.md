---
layout: post #always use this
title: Improved displacement estimation in homodyne Michelson interferometers  #This becomes the title of the page
date: 2018-04-27
categories: [nonlinear control, sliding mode]
---


Interferometry can be used to measure length displacements with high accuracy and resolution. Measuring length using interferometry relates the measurement directly to the definition of the meter, via the frequency $$ \omega = 2 \pi f $$, or wavelength $$\lambda$$, of the laser source used, since the two are related by 
$$
\begin{equation}
lambda= c/f
\end{equation} 
$$, 
where $$c$$ is the speed of light in vacuum. The accuracy of the measurement is therefore in principle only limited by how well the frequency of the laser source can be determined.

![SIOS SP-S Series]({{site.baseurl}}/assets/sp_s_series.png)


Displacement measurement using optical interferometry is mainly done using variants of the Michelson interferometer, using highly coherent and polarized light from a laser source. Resolution below 1 nm is routinely achieved in suitable environmental conditions, but the accuracy of the measurements are impacted due to several non-ideal effects. **Improved estimation methods can rectify these accuracy problems.**

![Michelson interferometer]({{site.baseurl}}/assets/michelson_optical_diagram_03.png)


* Learn how to use a SIOS laser interferometer to measure displacement (distance).
* Study optics and models of the homodyne Michelson interferometer.
* Study the methods currently used (e.g. the Heydemann-method) to determine displacement from the interference signals.
* Identify suitable estimation methods for estimating the parameters and signals in the model, such as the extended and unscented Kalman filter, and the particle filter.
* Look for ways to improve the modelling, to better capture non-ideal effects.
* Determine under what conditions the parameter and signal estimates converge, and how to improve convergence rate.
* Perform experiments using the SIOS laser interferometer to collect data.
* Compare current methods with you own method(s).
