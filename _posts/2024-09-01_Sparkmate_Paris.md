---
layout: post
title: "Project: Tracking Beacon"
author:
- Alvina
---

<b>Status:</b> Archived project for the UBC AeroDesign Team (Sensors and Controls Subteam)

## Quick Description
I worked on designing a closed-loop control system with stepper motors and encoders to control the movement of a tracking beacon; this beacon was supposed to point an antenna at our plane while it is flying. This project involved creating a set of requirements to select the optimal motors and encoders for our design, purchasing the components, soldering them together, and (currently) writing code to create a functioning closed-loop system.

## Materials Used

- Arduino Nano RP2040 connect
- Two stepper motors with built-in encoders [Exact Model](https://www.omc-stepperonline.com/p-series-nema-17-closed-loop-stepper-motor-48ncm-67-99oz-in-with-encoder-1000ppr-4000cpr-17e1k-05)
- Two Motor Drivers [Exact Model](https://components101.com/modules/drv8825-stepper-motor-driver-module)
- Salae Logic Pro Digital Logic Analyzer
- many other tiny electrical components
- Many, Many Websites

## Helpful Links for Explorers
- [Selecting a Motor Driver](https://community.robotshop.com/tutorials/show/how-to-make-a-robot-lesson-5-choosing-a-motor-controller)
- [How to Control a DC Motor with an Encoder](https://www.youtube.com/watch?v=dTGITLnYAY0&ab_channel=CurioRes)
- [AccelStepper Library](https://www.airspayce.com/mikem/arduino/AccelStepper/)
- [(pdf from Sparkfun) How to Use a Quadrature Encoder](https://cdn.sparkfun.com/datasheets/Robotics/How%20to%20use%20a%20quadrature%20encoder.pdf)
  
## Step By Step Playthrough

I was in charge of the electrical system for this project, and another mechanical engineering student on the same subteam was responsible for designing the physical beacon. 


This will not be a detailed walkthrough, but here are the general steps I used:
1. Research, research, and research. Understanding how encoders work, how stepper motors work, and how you can use one to control the other. All relevant links are included above.
2. Picking a motor that is strong enough to push the beacon's arm (according to calculations done by my fellow mechanical engineering student)
3. Once the motor was picked, I chose motor drivers that were strong enough to power the motors that I had chosen and had the correct increment size.
4. Designing the circuit that would connect all of the components together, including using any recommended circuits provided by their datasheets and corresponding websites. My hand-drawn schematic is shown below. 
5. Now came time to work on the code. I started from a very basic set of code and simply made my stepper motor take very slow steps and read the encoder output with the Digital Logic Analyzer.
<img src="/assets/images/tracking_beacon_schematic.png" style="width:60%">


  Unfortunately, while I was able to develop the control code for the motors, I was unable to make it work because of the really erratic behavior of the encoders. 
  With every step of the motor, the encoder would vibrate many times back and forth. No matter how many times I analyzed it, I could not determine a consistent pattern for the amount of times it would vibrate.
  And without a consistent pattern, I cannot properly control my motor because my code will not be able to accurately determine how many steps the motor actually took. 

Here is a sneak peak photo of my DLA output analyses:

<img src="/assets/images/encoder_analysis.png" style="width:60%">
