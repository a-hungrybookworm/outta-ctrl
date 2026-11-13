# Outta-Ctrl

A custom 64-key tactile mechanical keyboard designed from scratch - including a custom PCB, case, firmware, and even keycaps. 

<img width="1377" height="540" alt="Header_image" src="https://github.com/user-attachments/assets/9b48e887-3c2d-4cf5-8812-c64728dcfff7" />

## Features
* Custom PCB & layout
* 3D designed sandwich-mount case
* Custom RMK firmware
* Tactile MX-compatible switches
* Screw-in stabilisers
* Custom keycaps

## Components 
* Custom PCB
* 3D-printed case
* Tactile Gateron switches
* 1N4148 diodes
* Raspberry Pi Pico 
* Clear screw-in stabilizers
* Blank white (soon-to-be-doodled-on) keycaps

## Design Process
Initially, I planned the 64-key layout for my keyboard, and decided which components I would use. 

I then designed the PCB in KiCAD. I initially figured out which libraries/ footprints to use, connected them to form the keyboard matrix (row-to-col) and finally arranged the components and routed the traces.

Next, I learnt how to 3D model in Onshape, while simultaneously modelling the [case](https://cad.onshape.com/documents/6f7a7e00666188f7ad4cf98b/w/f1435142402e02a68e5f24dd/e/d5e9a1b6849998dde5a38184). I used a sandwich mount for its simplicity, but ended up removing the top (above the plate) to cut costs, and split the case as it was too big for the bed size. 

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


 __Plate__:

<img width="1354" height="545" alt="Plate" src="https://github.com/user-attachments/assets/b8aab294-1011-464b-ab19-800f72fbe7cd" />

 __Base__:

<img width="1475" height="617" alt="Base" src="https://github.com/user-attachments/assets/868f2eb9-90bd-4c9d-a6be-6ae7c7365ebe" />

__Assembly__:

(without all keycaps/ stabs)

<img width="1302" height="552" alt="Assembly" src="https://github.com/user-attachments/assets/de8ac19b-dd45-41ae-b490-16fe86362277" />

## Bill of Materials (BOM)

| SI No. | Name | Notes | Quantity | Price / Unit (INR) | Shipping (INR) | Total (INR) | Running Total (INR) | Price/Unit (USD) | Total (USD) | Running Total (USD) | Link | Vendor |
| --- | --- | --- | --- | ---: | ---: | ---: | ---: | ---: | ---: | ---: | --- | --- |
| 1 | Gateron G Pro 3.0 Brown Tactile Switches (Pack of 10) | MX-compatible Switches | 7 | 190 | 0 | 1330 | 1330 | 2.02 | 14.15 | 14.15 | [Switch](https://stackskb.com/store/gateron-g-pro-3-0-brown-ks-9-tactile-switch-pack-of-10/) | StacksKB |
| 2 | PCB (manufactured by Robu) | Manufactured by Robu | 5 | 1066 | 0 | 5330 | 6660 | 11.34 | 56.70 | 70.85 | [PCB_Robu](https://github.com/a-hungrybookworm/outta-ctrl/blob/main/BOM/PCB%20Order.png) | Robu |
| 3 | Durock Clear Screw-In Stabilizers V2 | Screw-in stabilisers | 1 | 1650 | 0 | 1650 | 8310 | 17.55 | 17.55 | 88.40 | [Stabs](https://stackskb.com/store/durock-clear-screw-in-stabilizers-v2/) | StacksKB |
| 5 | 1N4148 Diodes | Keyboard matrix | 65 | 1.07 | 49 | 118.55 | 8428.55 | 0.01 | 1.26 | 89.67 | [Diodes](https://robu.in/product/1n4148-onsemi-100v-1v10ma-4ns-200ma-do-35-switching-diodes-rohs/) | Robu |
| 6 | Raspberry Pi Pico | MCU | 1 | 384 | 0 | 384 | 8812.55 | 4.09 | 4.09 | 93.75 | [Pico](https://robu.in/product/raspberry-pi-pico/) | Robu |
| 7 | Heat Set Threaded Round Female Insert Nut | M3x6mm, pack of 5 | 2 | 15 | 60 | 90 | 8902.55 | 0.16 | 0.96 | 94.71 | [Heat Set Insert](https://makerbazar.in/products/brass-heat-set-threaded-round-female-insert-nut?variant=48339035554032) | Makerbazar |
| 8 | M3 X 10mm Phillips Pan head SS 304 Screw | M3x10mm | 8 | 1.80 | 69 | 83.40 | 8985.95 | 0.02 | 0.89 | 95.60 | [Screws](https://onlyscrews.in/products/phillips-pan-head-m3-x-10mm-pack-of-20?currency=INR&country=IN&variant=48468583874873) | Only Screws |
| 9 | Blank White Cherry Profile Keycaps | For later customization | 1 | 1000 | 0 | 1000 | 9985.95 | 10.64 | 10.64 | 106.23 | [Keycaps](https://stackskb.com/store/stackspbt-blank-white-cherry-profile-keycaps-113-key/) | StacksKB |
| 10 | 7u Spacebar | Custom key | 1 | 300 | 0 | 300 | 10285.95 | 3.19 | 3.19 | 109.43 | [Spacebar](https://curiositycaps.in/products/7u-spacebar-replacement-key) | CuriosityCaps |
| 11 | 3D Print | Case! | 1 | 1333.86 | 100 | 1433.86 | 11719.81 | 14.19 | 15.25 | 124.68 |  | Printing Legion |
|  | **Total (with shipping)** |  |  |  |  |  |  |  |  | **124.68** |  |  |

**Exchange rate used:** ₹94 ≈ $1  
**Grand total:** ₹11,719.81 / **$124.68**

## Credits
This project was made possible through open-source hardware and design resources, and continuous support from the mechanical keyboard community. A special thank-you to the Hackclub YSWS Keeb, for inspiring me to take up this project, guiding me along the way, and most importantly, funding this project.
