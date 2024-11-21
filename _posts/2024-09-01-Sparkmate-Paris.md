---
layout: post
title: "Projects as a Product Engineer at Sparkmate Paris"
author:
- Alvina
---

## Quick Description
I did a 4-month co-op at the Sparkmate Paris office from May - September of 2024. Sparkmate is an engineering consulting company that builds unique, innovative mechanical and electrical projects. 

## Oria Marine VDR

Oria Marine and Sparkmate collaborated to make a box that monitored boat fuel-efficiency, and displayed other statistics. These boxes were used during the Paris 2024 Olympics at the sailing competition in Marseilles, France! To read more about Oria Marine, visit their home page here: [Oria Marine] (https://www.oria-marine.com/). 

For this product, I worked on two projects. One was developing a prototype firmware that would track the force and frequency of the impacts that the boat would experiene while on the water. The second project was working on the main, existing firmware of Oria Marine and fixing several large issues that prevented the code from running. The firmware was written in C++ and utilized RTOS, both of which I was not familiar with prior to the project. Debugging RTOS firmware is much more difficult than debugging software because it is challenging to step through real-time dependent code. And becuase the product was on a PCB and utilized almost all of the microcontroller pins, JTAG debuggers were not an option. 

Working on existing firmware is challenging in its own way, because it is code that somebody else had written. The previous engineer that had created this code was no longer at the company, so I had limited help in understanding the software. However, I succesfully familiarized myself with the firmware by carefully reading through the documentation, making flow charts of the firmware, and tinkering with the functions to fully understand the functionality before attempting to fix the major existing bugs. I then used creative techniques to narrow down where the issues were in the firmware, and single-handedly developed fixes for the issues. I worked over 80 hours in one week in order to have the product ready for testing and deployment so that it would be ready in time.

I also helped debug and fix the physical boxes themselves. Types of issues included, poor sim card reading, broken batteries, overheating components, and etc. 

Part of testing and debugging this product involved going to the Olympic sailing site and mounting the boxes in the boats, then running the boats to see if the box behaved as predicted. Below are some photos of me during those visits! 

<img src="/assets/images/olympics_sailing_picture.JPG" style="width:60%">
<img src="/assets/images/oria_testing.jpg" style="width:60%">
<img src="/assets/images/oria_mounted.jpg" style="width:60%">

<p>
 <div class="row">
    <img src="/assets/images/olympics_sailing_picture.JPG" style="width:30%">
    <img src="/assets/images/oria_testing.jpg" style="width:30%">
    <img src="/assets/images/oria_mounted.jpg" style="width:30%">
</div> 
</p>

