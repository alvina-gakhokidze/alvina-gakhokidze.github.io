---
layout: post
title: "Projects as a Product Engineer at Sparkmate Paris"
author:
- Alvina
---

## Quick Description
I did a 4-month co-op at the Sparkmate Paris office from May - September of 2024. Sparkmate is an engineering consulting company that builds unique, innovative mechanical and electrical projects. 

## Oria Marine VDR

Oria Marine and Sparkmate collaborated to make a box that monitored boat fuel-efficiency, and displayed other statistics. These boxes were used during the Paris 2024 Olympics at the sailing competition in Marseilles, France! To read more about Oria Marine, visit their home page here: [Oria Marine](https://www.oria-marine.com/). 

For this product, I worked on two projects. One was developing a prototype firmware that would track the force and frequency of the impacts that the boat would experiene while on the water. The second project was working on the main, existing firmware of Oria Marine and fixing several large issues that prevented the code from running. The firmware was written in C++ and utilized RTOS, both of which I was not familiar with prior to the project. Debugging RTOS firmware is much more difficult than debugging software because it is challenging to step through real-time dependent code. And becuase the product was on a PCB and utilized almost all of the microcontroller pins, JTAG debuggers were not an option. 

Working on existing firmware is challenging in its own way, because it is code that somebody else had written. The previous engineer that had created this code was no longer at the company, so I had limited help in understanding the software. However, I succesfully familiarized myself with the firmware by carefully reading through the documentation, making flow charts of the firmware, and tinkering with the functions to fully understand the functionality before attempting to fix the major existing bugs. I then used creative techniques to narrow down where the issues were in the firmware, and single-handedly developed fixes for the issues. I worked over 80 hours in one week in order to have the product ready for testing and deployment so that it would be ready in time.

I also helped debug and fix the physical boxes themselves. Types of issues included, poor sim card reading, broken batteries, overheating components, and etc. 

Part of testing and debugging this product involved going to the Olympic sailing site and mounting the boxes in the boats, then running the boats to see if the box behaved as predicted. Below are some photos of me during those visits! 

<p>
 <div class="row">
    <img src="/assets/images/olympics_sailing_picture.JPG" style="width:30%">
    <img src="/assets/images/oria_testing.jpg" style="width:30%">
    <img src="/assets/images/oria_mounted.jpg" style="width:30%">
</div> 
</p>

## Murfy Motherboard

Murfy and Sparkmate collaborated to create a service that will refurbish broken washing machines in order to combat waste in France. It is an excellent environmentally-friendly business, and you can read more about them here: [Murfy](https://murfy.fr/). 

For this project, I helped create version 4 of the motherboard for the washine machines. This involved understanding the design decisions behind the previous versions, discussing additional technological needs for the new revision, and identifying areas of improvement. I created comparison tables to choose any major new equipment like microcontrollers and digital ICs for the new PCB. I designed the new schematic, specced materials, and performed revisions based on mentor feedback to perfect the circuit. I also performed work on the physical layout of the PCB, however my internship ended before I could finalize the layout. 

Designing this PCB helped me familiarize myself with practical applications of many electrical engineering theories that we have learned but didn't apply - for example, filters and transistors- and also was a great learning opportunity on developing circuits for microcontroller chips, as opposed to buying already prepared dev boards. To design this PCB, I used KiCad.

For privacy, I cannot post photos of the schematics or my work, but you can see me in the picture below standing next to the ad for the company in the Parisi metro! 

 <img src="/assets/images/Murfy_Ad.JPG" style="width:60%">

