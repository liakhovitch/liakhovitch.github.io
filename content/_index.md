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

## CRÖNCH: Not-Entirely-Sane Digital Delay Pedal

Crönch is a hardware audio effects processor, inspired by the Sonic Charge Permut8 software plugin. The device is based on an RP2040 MCU and performs 192KHz audio processing in real time, while driving 76 LEDs and 48 switches with a second processor core. I assembled it by hand and soldered SMD components with a homemade oven. This project is currently on pause, but it still represents my best work to-date - especially the [schematic](https://github.com/liakhovitch/cronch/blob/main/pcb/effectpedal/fabrication/schematic.pdf). More info available on [Github](https://github.com/liakhovitch/cronch).

<img src='public/images/cronch.jpg'><br/><br/>

## Undergrad Senior Capstone: CAN Logger

I was part of a four-person team that developed an automotive diagnostic bus (CAN) logging appliance for Hyster-Yale inc. We worked on this in the middle of the parts shortage, so we chose a somewhat underpowered single-core Cortex M4 microcontroller due to its wide availability. As the firmware lead, I was tasked with developing performant real-time firmware that could make hard data integrity guarantees when receiving at maximum bus speed. More info (including a detailed technical report) available on the [OSU EECS project showcase](https://eecs.engineering.oregonstate.edu/project-showcase/projects/?id=gSDrxXntCfJTY05l).

<img src='public/images/canlogger.jpg'><br/><br/>

## Junior Capstone: Egg Timer

My junior capstone class tasked me with bringing a product from concept to prototype in ten weeks, by myself. I built a digital kitchen timer, with my very first custom PCB and a CNC-machined acrylic enclosure. The timer is based on the widely available STM32f103 32-bit MCU. I try to learn as much as possible from every academic project, so I wrote the firmware in Rust with the experimental (at the time) realtime interrupt-based concurrency (RTIC) framework. More info available on the [OSU EECS project showcase](https://eecs.engineering.oregonstate.edu/project-showcase/projects/?id=trLHRkyRlfQhVEzy) and [Github](https://github.com/liakhovitch/junior_design).
<img src='public/images/eggtimer.jpg'><br/><br/>

## Microcontroller System Design Class: Another Clock

This is an alarm clock (AVR, firmware in C) that I built for Dr. Roger Traylor's MCU System Design class in early 2023. We were tasked with developing a different part of the clock each week. Most students ended up with a fragile mess of three or more breadboards, but I planned ahead and used perfboard. This class effectively simulated a rapid prototyping environment with stringent and constantly expanding requirements. As per OSU policy, the firmware cannot be published but is available upon request.

<img src='public/images/alarmclock.jpg'><br/>
<img src='public/images/spaghetti.jpg'><br/><br/>

## Hacking an IoT Sensor

In my IT job at OSU, I came across a research group that was locked out of their $10,000 fleet of remote sensors when the manufacturer went bankrupt and shut down their cloud services. By the end of the day, I gained root access and restored functionality to the devices. The exploit involved a TFTP misconfiguration which made it possible to retrieve the hashed root password, and a weak root password that was easily crackable.

<img src='public/images/sensor.jpg'><br/><br/>

## Google Bug Bounty

I stumbled upon an issue where the Google Home mobile app would crash while setting up a Google Home smart speaker. After extensive toubleshooting, I determined that this only happened whenever a wireless network with a quotation symbol in the SSID was present. I recognized this as a potential zero-click code injection vulnerability, so I reported it to the bug bounty program and received a $500 reward.

<img src='public/images/home.jpg'><br/><br/>

## HOOT: Owl-Shaped Emergency Radio

In early 2022, I made my friend a pair of owl-shaped LoRa radios as a housewarming present. Tapping one owl would make the other hoot, allowing for simple communication around the house ("Hoot, dinner is ready!"). In an emergency situation, the watertight electronics enclosures could be taken out of their owl shells and used to transmit morse code, or paired with a smartphone (via adhoc WiFi) to transmit text. HOOT is based on an ESP32 MCU with firmware in C, and implements LoRa communication, ad-hoc WiFi, a web server, speech synthesis, audio sample playback, and an integrated battery. This was all rapidly constructed over the course of one month. The hastily-written firmware is unfit for publication, but there is a [manual](public/hoot_manual.pdf).

<img src='public/images/hoot.jpg'><br/><br/>

## Laser Tag Proximity Mine

In 2018, I felt like experimenting with the FORTH programming language. I reverse-engineered the infrared communication protocol used by a set of Hasbro laser tag blasters, then made a compatible proximity mine. The mine includes features such as IFF beacon transmission, automatic detection of the user's team, configurable damage, and more. Firmware is available on [Github](https://github.com/liakhovitch/claymore).

<img src='public/images/claymore.jpg'><br/><br/>

## Router Storage Expansion

During my freshman year at OSU, I had a hobby of buying dirt-cheap used routers and repurposing them as general-purpose single-board computers. One particular device came with only 4MB of storage and no USB port. I found that the onboard SOC included USB support, so I glued an 8GB flash drive to the board and ran jumpers from the data pins directly to the SOC's QFN package. I then had to compile OpenWRT (a Linux distro for routers), with a custom kernel that included USB/storage drivers and practically nothing else. From there, I could set up the device to load further data from the flash drive.

<img src='public/images/router.jpg'><br/><br/>
