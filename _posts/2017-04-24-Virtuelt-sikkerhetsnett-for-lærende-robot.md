---
layout: post #always use this
title: Virtuelt sikkerhetsnett for lærende robot   #This becomes the title of the page
date: 2017-04-24
categories: [nonlinear control, sliding mode]
---
# Virtuelt sikkerhetsnett for lærende robot #
 
I Neodroid-prosjektet skal en robot lære ved prøving og feiling, ved bruk av reinforcement learning. For at dette skal kunne gjøres på en sikker måte trenger roboten et virtuelt sikkerhetsnett som hindrer at den skader seg selv eller omgivelsene.
 
Det virtuelle sikkerhetsnettet innbefatter:
* Unngå selvkollisjon, også med griper montert på.
* Unngå kollisjon med objekter skannet med 3D kamera av typen Intel RealSense.
* Avgjøre om en bevegelsesbane for robotens endeffektor vil forårsake kollisjon.
* I begge tilfeller gi robotens styringsprogram tilbakemelding om type kollisjon som ble unngått.
 
Studenten skal jobbe sammen med en PhD-kandidat i prosjektet, som skal implementere reinforcement learning.

Kontaktperson: John.Reidar.Mathiassen@sintef.no
