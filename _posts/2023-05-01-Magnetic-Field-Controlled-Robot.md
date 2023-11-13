---
layout: post
title: "Project: Magnetic Field-Controlled Robot"
author:
- Alvina
---

<p>Status:</p> Completed Electrical Project for ELEC 291, a course at UBC

## Quick Description
The goal of this project was to design a magnetic field-controlled robot. It consists of two parts - are transmitter with two big inductors, and a receiver (the car). 
Our professor provided some schematics and code, but the challenge of this project was to <em>integrate</em> everything and <em>complete</em> code. 

The car had two modes:
* Controller Mode - receiving commands from the receiver to turn left/right, move backward/forwards, and turn backward left/backward right
* Tracking Mode - follow the receiver in any direction that it is moved, maintaining an exact distance of 50cm. 

## Materials Used
- PIC32MX130 microcontroller 
- STM32L051 microcontroller
- MOSFET drivers
- M8275-ND Inductors
- many other tiny electrical components


## Step By Step Playthrough


I was the leader of the 6 student team that worked on this project. We delegated tasks between the students - 3 working on the transmitter and 3 (including me) working on the receiver (the car). Both microcontrollers were programmed in C. 

### My work on the transmitter included:
<b>Constructing the H-bridge.</b>
Because there is limited space on the car shell, we had to condense our circuit onto one breadboard - which meant the H-bridge had to be incredibly condensed. Here is a photo of the H-bridge I built:

<img src="/assets/images/hbridge.jpg" style="width:60%">

Then, we had to integrate the rest of the components: including the inductors that receive the signal from the transmitter, and the microcontroller that receives the signal, interprets it, and then controls the H-bridge. 
This is what it initially looked like:

<img src="/assets/images/initial_car.jpg" style="width:60%">

We tested each of the components individually before combining them (a lesson we learned from our past big project, where we did NOT do that...).

Unfortunately, the inductors were receiving a very weak signal. We tested the receiver, and the measured voltage was exactly what it was supposed to be. This meant there was a problem with the inductors on the receiver, but we could not change them. 

Our solution was to add cascaded amplifiers on the receiver - this required a lot of trial and error to determine how much we needed to amplify the signal. This is the messy final version of the car:


<img src="/assets/images/final_car.jpg" style="width:60%">

As part of the project, we were required to make a video (or write an essay) about this project. You can see my teammate's (Ruth Tao) video on YouTube by clicking on the image below:
[![Video of Magnetic Field Controlled Robot](/assets/images/picture_of_testing_car.jpg)](https://www.youtube.com/watch?v=LQKEylR-Bv8&ab_channel=RuthTau)





