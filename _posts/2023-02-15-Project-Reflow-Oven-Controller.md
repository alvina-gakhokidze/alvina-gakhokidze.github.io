---
layout: post
title: "Project: Reflow Oven Controller"
categories: art
author:
- Alvina
---

<b>Status:</b> Completed Electrical Project for ELEC 291, a course at UBC. <b>Role:</b> Co-Leader. 

## Quick Description

The goal of this project was to design a reflow oven controller (typically used for soldering SMD components onto PCBs), coded completely in <b>8051 Assembly.</b>

The controller sends PWM signals to control a solid-state relay box that is hooked up to a toaster oven. The controller managed the temperature rise, pause, and cool-down, and had a temperature sensor to ensure that the oven was behaving accordingly. 

The buttons controlled the parameters of the reflow process, and we had audio output on the speaker that indicated the different "milestones" the oven achieved as it was going through the reflow process. 

We used finite state machines written in 8051 Assembly to control the pwm signals to the SSR:

We initially implemented PWM by configuring a timer for PWM mode. But afterward, our professor released example code that showed us how to do PWM in an easier and more intuitive way, and as we were struggling to figure out how to actually get the right output with the previous idea, we decided to study his basic template. His code gave us the idea of generating PWM by manually setting a pin on the microcontroller high/low inside of a timer using specific flags. 

We took that basic idea and worked on the logic required to make a changing PWM signal requiring different power ratios. As for the PWM finite state machine, we debated on initially simply changing the timer configuration after a certain temperature/time was reached by checking for it each time we entered the main loop. But, with the professors guidance, we realized it would be better to actually use a finite state machine, and use flags to keep our system in individual states so that we wouldn’t have to cycle through a large loop.

## Primary Concepts/Tools Used in this Project

* 8051 Assembly
* Finite State Machines
* Circuit Design and Debugging
* Pulse Coded Modulation
* Interrupts, Timers, etc. in Assembly.

Here is a photo of the final breadboard. Unfortunately, I did not take a video of how this project worked :(

<img src="/assets/images/reflow_oven_2.jpg" style="width:60%">
  



