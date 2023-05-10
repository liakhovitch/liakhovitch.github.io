+++
title = "Home"
template = "section.html"
+++

# Anton Liakhovitch
*Embedded Software Engineer*  
aeliakhovitch@gmail.com, 971-295-0315  

---
<br/>
<h1 style="text-align: center;"><i>Projects</i></h1>

<br/>

## CRÖNCH: Not-Entirely-Sane Audio Effects Unit

Crönch is a hardware audio effects processor, inspired by the Sonic Charge Permut8 software plugin. The device is based on an RP2040 MCU and performs 192KHz audio processing in real time, while driving 76 LEDs and 48 switches with a second processor core. I assembled it by hand, and soldered SMD components with a homemade oven. This project is currently on pause, but it still represents my best work to-date - especially the [schematic](https://github.com/liakhovitch/cronch/blob/main/pcb/effectpedal/fabrication/schematic.pdf). More info on [Github](https://github.com/liakhovitch/cronch).

<img src='images/cronch.jpg'><br/><br/>

## Undergrad Senior Capstone: CAN Logger

I was part of a four-person team that developed an automotive diagnostic bus (CAN) logging appliance for Hyster-Yale inc. We worked on this in the middle of the parts shortage, so we chose a somewhat underpowered single-core Cortex M4 microcontroller due to its wide availability. As the firmware lead, I was tasked with developing performant real-time firmware that could make hard data integrity guarantees when receiving at maximum bus speed. More info (including a detailed technical report) on the [OSU EECS project showcase](https://eecs.engineering.oregonstate.edu/project-showcase/projects/?id=gSDrxXntCfJTY05l).

<img src='images/canlogger.jpg'><br/><br/>

## Junior (Solo) Capstone: Egg Timer

My junior capstone class tasked me with bringing a product from concept to prototype in ten weeks, by myself. I built a digital kitchen timer, with my very first custom PCB and a CNC-machined acrylic enclosure. The timer is based on the widely available STM32f103 32-bit MCU. I try to learn as much as possible from every academic project, so I wrote the firmware in Rust with the experimental (at the time) realtime interrupt-based concurrency (RTIC) framework. More info available on the [OSU EECS project showcase](https://eecs.engineering.oregonstate.edu/project-showcase/projects/?id=trLHRkyRlfQhVEzy) and [Github](https://github.com/liakhovitch/junior_design).
<img src='images/eggtimer.jpg'><br/><br/>

## Microcontroller System Design Class: Another Clock

This is an alarm clock (AVR, firmware in C) that I built for Dr. Traylor's MCU System Design class in early 2023. We were tasked with developing a different part of the clock each week. Most students ended up with a fragile mess of three or more breadboards, but I planned ahead and used perfboard. This class effectively simulated a rapid prototyping environment with stringent and constantly expanding requirements. As per OSU policy, the firmware cannot be published but is available upon request.

<img src='images/alarmclock.jpg'><br/>
<img src='images/spaghetti.jpg'><br/><br/>

## Hacking an IoT Sensor

In my IT job at OSU, I came across a research group that was locked out of their $10,000 fleet of remote sensors when the manufacturer went bankrupt and shut down their cloud services. By the end of the day, I gained root access and restored functionality to the devices. The exploit involved a TFTP misconfiguration which made it possible to retrieve the hashed root password, and a weak root password that was easily crackable.

## Google Bug Bounty

I stumbled upon an issue where the Google Home mobile app would crash while setting up a Google Home smart speaker. After extensive toubleshooting, I determined that this only happened whenever a wireless network with a quotation symbol in the SSID was present. I recognized this as a potential zero-click code injection vulnerability, so I reported it to the bug bounty program and received a $500 reward.
