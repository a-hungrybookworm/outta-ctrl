# Outta-Ctrl

A custom 64-key linear mechanical keyboard designed from scratch - including a custom PCB, case, firmware, and even keycaps. 

<img width="1537" height="630" alt="__" src="https://github.com/user-attachments/assets/ef7ff690-19a9-4dea-931b-8e4d6d028068" />

## Features
* Custom PCB & layout
* 3D designed sandwich-mount case
* Custom RMK firmware
* Hotswappable MX-compatible switches
* Screw-in stabilisers
* Custom keycaps

## Components 
* Custom PCB
* 3D-printed case
* MX-compatible switches
* 1N4148 diodes
* Raspberry Pi Pico 
* Hotswap sockets
* Clear screw-in stabilizers
* Blank white (soon-to-be-doodled-on) keycaps

## Design Process
Initially, I planned the 64-key layout for my keyboard, and decided which components I would use. 

I then designed the PCB in KiCAD. I initially figured out which libraries/ footprints to use, connected them to form the keyboard matrix (row-to-col) and finally arranged the components and routed the traces.

Next, I learnt how to 3D model in Onshape, while simultaneously modelling the case. I used a sandwich mount for its simplicity, and split the case into two mutually screwable sections, as it was too big for the bed size. This will help in easy assembly and disassembly.

Finally, I wrote the RMK firmware, which I will flash to my Pi Pico to control the keyboard.

## Why I built it
I've been fascinated by understanding how most everyday objects work, and when I saw a HackClub programme offering to teach me how to build one of them, a keyboard, I was thrilled. Finally, I had the opportunity to learn how to design keyboard PCBs, model their cases, write their custom firmware, and deeply understand how these devices function.

## Challenges
While designing the keyboard, I found several tasks challenging, such as
* understanding the specifications and limitations of the different components
* accounting for all the specific holes and features of the components while designing the 3D models
* finding footprints/ 3D models for my components
* finding keycaps for my design size

## What I learnt
I started this ambitious project with no experience at all, and only a list of tutorials (credit to [Keeb](keeb.hackclub.com)). Now, I've learnt so much, including (sequentially) - 
* how Github repositories function 
* how to write in Markdown, and how to write a readme
* how to design a PCB in KiCAD
* the matrix layout/schematic required for keyboard PCBs
* how to use Onshape for 3D designing
* the different keyboard mounting styles, and parts of a case
* what keyboard firmware does, and how to write it
* about different keyboard components, and their functions

## Images 

__Schematic__:

<img width="1292" height="706" alt="Schematic" src="https://github.com/user-attachments/assets/95da6ae8-050a-4e0c-8f9e-c86b718c7220" />


__Routed PCB__: 

 <img width="1219" height="444" alt="Routed" src="https://github.com/user-attachments/assets/b0076d37-0862-4ace-8045-c0773ef839b3" />

**3D Models:**

 __Top(Case)__:
 
<img width="1632" height="766" alt="Top" src="https://github.com/user-attachments/assets/1ab4260d-6302-4194-9b79-e992b298a52c" />

 __Plate__:

<img width="1680" height="708" alt="Plate" src="https://github.com/user-attachments/assets/9d4ca010-05ea-421d-a86f-7c7712748721" />

 __Base__:

<img width="1719" height="713" alt="Base" src="https://github.com/user-attachments/assets/144a5f8f-3c9c-460e-9547-a6692d863070" />

__Assembly__:

(without all keycaps/ stabs)

<img width="1537" height="630" alt="Assembly" src="https://github.com/user-attachments/assets/e9bf28a7-8f30-4788-9347-7950a1667eee" />

## Bill of Materials

| SI No. | Name | Notes | Quantity | Price Per Unit | Total | Running Total | Price/Unit(USD) | Total (USD) | Running Total (USD) | Link |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | Keygeek x MZ Y1 Keyboard Switch (Pack of 10) | MX-compatible Switches | 7 | 300 | 2100 | 2100 | 3.16 | 22.11 | 22.11 | [Switch](http://stackskb.com/store/keygeek-y1-keyboard-switch/) |
| 2 | PCB (manufactured by Robu) | Manufactured by Robu | 5 | 1062 | 5310 | 7410 | 11.18 | 55.89 | 78 | [PCB_Robu](https://github.com/a-hungrybookworm/outta-ctrl/blob/main/BOM/PCB%20Order.png) |
| 3 | Durock Clear Screw-In Stabilizers V2 | Screw-in stabilisers | 1 | 1650 | 1650 | 9060 | 17.37 | 17.37 | 95.37 | [Stabs](http://stackskb.com/store/durock-clear-screw-in-stabilizers-v2/) |
| 4 | Gateron Hotswap Sockets | Hotswap Sockets | 64 | 10 | 640 | 9700 | 0.11 | 6.74 | 102.11 | [Hotswap Switches](http://stackskb.com/store/gateron-hotswap-sockets/) |
| 5 | 1N4148 Diodes | Pack of 100, TH | 1 | 180 | 180 | 9880 | 1.89 | 1.89 | 104 | [Diodes](https://www.flipkart.com/elph-zener-diode-1n4148-pieces-100-electronic-components-hobby-kit/p/itmff7b2uhf4yng4) |
| 6 | Raspberry Pi Pico | MCU | 1 | 384 | 384 | 10264 | 4.04 | 4.04 | 108.04 | [Pico](https://robu.in/product/raspberry-pi-pico/) |
| 7 | Heat Set Threaded Round Female Insert Nut | M3, pack of 5 | 2 | 15 | 30 | 10294 | 0.16 | 0.32 | 108.36 | [Heat Set Insert](https://makerbazar.in/products/brass-heat-set-threaded-round-female-insert-nut?variant=48339035554032) |
| 8 | Philips Head Nuts & Bolts Set | M3, pack of 10 | 1 | 25 | 25 | 10319 | 0.26 | 0.26 | 108.62 | [Screws](https://makerbazar.in/products/philips-head-nuts-bolts-set-silver-plated-pack-of-10?variant=43604554383600) |
| 9 | Blank White Cherry Profile Keycaps | For later customization | 1 | 1000 | 1000 | 11319 | 10.53 | 10.53 | 119.15 | [Keycaps](https://stackskb.com/store/stackspbt-blank-white-cherry-profile-keycaps-113-key/) |
| 10 | 7u Spacebar | Custom key | 1 | 300 | 300 | 11619 | 3.16 | 3.16 | 122.31 | [Spacebar](https://curiositycaps.in/products/7u-spacebar-replacement-key) |

## Credits
This project was made possible through open-source hardware and design resources, and continuous support from the mechanical keyboard community. A special thank-you to the Hackclub YSWS Keeb, for inspiring me to take up this project, guiding me along the way, and most importantly, funding this project.
