# outta-ctrl

A 64-key linear mechanical keyboard, custom designed from the PCB to the keycaps.

## Features
* Custom 64-key PCB, case
* Custom firmware flashing
* Hotswap sockets
* Custom keycaps

## Why I built it
I've always been fascinated by those fancy, raised, clackety keyboards - and when I saw a HackClub programme offering to teach me how to build one, I was thrilled. I finally had the opportunity to learn how keyboards work (you know, one of those questions that keep you awake at night), and make my very own custom one, with the keys I like, and with custom keycaps I get to doodle on.

## Design Process
I first had to design a 64-key layout for my keyboard, and plan the components I would be using. I then designed the PCB in KiCAD - first adding and connecting the correct footprints on the schematic, then arranging and routing the traces. I then designed a case (sandwich mount) on Onshape, for easy disassembly and assembly. Finally, I wrote the RMK firmware, which I will flash to my keyboard.

## Components 
* Custom PCB
* 3D-printed case
* MX-compatible switches
* 1N4148 diodes
* Raspberry Pi Pico 
* Hotswap sockets
* Clear screw-in stabilizers
* Blank white (soon-to-be-doodled-on) keycaps

## Files
The PCB fabrication files can be accessed at [Gerbers](https://github.com/a-hungrybookworm/outta-ctrl/tree/main/PCB_Fabrication), and the Onshape document at [3D-Design](https://cad.onshape.com/documents/6f7a7e00666188f7ad4cf98b/w/f1435142402e02a68e5f24dd/e/d5e9a1b6849998dde5a38184)

## What I learnt
I started this ambitious project with no experience at all, and only a list of tutorials (credit to keeb.hackclub.com). Now, I've learnt so much, such as - (I've arranged it sequentially)
* how Github repositories function
* how to write a readme, or markdown
* how to design a PCB
* the layout/schematic required for keyboards
* how to 3D design (in Onshape)
* the different keyboard mounting styles, and parts of a case
* what keyboard firmware does, and how to write it
* a lot of nerdy info on different keyboard components

## Challenges
I faced several minor issues while designing the keyboard, such as finding footprints/ 3D models for my components, and especially finding keycaps for my design sizes. Anticipating the challenges I'm going to face while building the keyboard, though, I think I'll fill this part later.

## Images 

__Schematic__:

<img width="1292" height="706" alt="Schematic" src="https://github.com/user-attachments/assets/95da6ae8-050a-4e0c-8f9e-c86b718c7220" />


__Routed PCB__: 

 <img width="1219" height="444" alt="Routed" src="https://github.com/user-attachments/assets/b0076d37-0862-4ace-8045-c0773ef839b3" />

*3D Models:* 

 __Top(Case)__:
 
<img width="1632" height="766" alt="Top" src="https://github.com/user-attachments/assets/1ab4260d-6302-4194-9b79-e992b298a52c" />

 __Plate__:

<img width="1680" height="708" alt="Plate" src="https://github.com/user-attachments/assets/9d4ca010-05ea-421d-a86f-7c7712748721" />

 __Base__:

<img width="1719" height="713" alt="Base" src="https://github.com/user-attachments/assets/144a5f8f-3c9c-460e-9547-a6692d863070" />

__Assembly__:

*(without all keycaps/ stabs)*

<img width="1537" height="630" alt="Assembly" src="https://github.com/user-attachments/assets/e9bf28a7-8f30-4788-9347-7950a1667eee" />

## BOM
| SI No. | Name | Notes | Quantity | Price Per Unit | Total | Running Total | Price/Unit (USD) | Total (USD) | Running Total (USD) | Link |
| --- | --- | --- | --- | --- | --- | --- | --- | --- | --- | --- |
| 1 | Keygeek x MZ Y1 Keyboard Switch (Pack of 10) | MX-compatible Switches | 7 | 300 | 2100 | 2100 | 3.16 | 22.11 | 22.11 | [Switch](http://stackskb.com/store/keygeek-y1-keyboard-switch/) |
| 2 | PCB (Robu) | 5 is the min. order quantity | 5 | 1062 | 5310 | 7410 | 11.18 | 55.89 | 78.00 | [PCB_Robu](https://github.com/a-hungrybookworm/outta-ctrl/blob/main/BOM/PCB%20Order.png) |
| 3 | Durock Clear Screw-In Stabilizers V2 | Screw-in stabilisers | 1 | 1650 | 1650 | 9060 | 17.37 | 17.37 | 95.37 | [Stabs](http://stackskb.com/store/durock-clear-screw-in-stabilizers-v2/) |
| 4 | Gateron Hotswap Sockets | Hotswap Sockets | 64 | 10 | 640 | 9700 | 0.11 | 6.74 | 102.11 | [Hotswap Switches](http://stackskb.com/store/gateron-hotswap-sockets/) |
| 5 | 1N4148 Diodes | Pack of 100, TH | 1 | 180 | 180 | 9880 | 1.89 | 1.89 | 104.00 | [Diodes](https://www.flipkart.com/elph-zener-diode-1n4148-pieces-100-electronic-components-hobby-kit/p/itmff7b2uhf4yng4) |
| 6 | Raspberry Pi Pico | MCU | 1 | 384 | 384 | 10264 | 4.04 | 4.04 | 108.04 | [Pico](https://robu.in/product/raspberry-pi-pico/?gad_source=4&gad_campaignid=19974686076&gbraid=0AAAAADvLFWdAl5Wi83k9ojkIRV64IGicN&gclid=Cj0KCQjw2OnUBhC2ARIsACKyfaE3Ny_Zh17xOpxe-m0kUq52dTaldignAKoolyYla7WaLtCoqZ6H4d4aAi2KEALw_wcB) |
| 7 | Heat Set Threaded Round Female Insert Nut | M3, pack of 5 | 2 | 15 | 30 | 10294 | 0.16 | 0.32 | 108.36 | [Heat Set Insert](https://makerbazar.in/products/brass-heat-set-threaded-round-female-insert-nut?variant=48339035554032) |
| 8 | Philips Head Nuts & Bolts Set | M3, pack of 10 | 1 | 25 | 25 | 10319 | 0.26 | 0.26 | 108.62 | [Screws](https://makerbazar.in/products/philips-head-nuts-bolts-set-silver-plated-pack-of-10?variant=43604554383600) |
| 9 | Blank White Cherry Profile Keycaps | For later customization | 1 | 1000 | 1000 | 11319 | 10.53 | 10.53 | 119.15 | [Keycaps](https://stackskb.com/store/stackspbt-blank-white-cherry-profile-keycaps-113-key/) |

## Credits
This project was made possible by a multitude of open-source hardware, and design resources, and continuous support from the mechanical keyboard community. A special thank-you to the Hackclub YSWS Keeb, for inspiring me to take up this project and helping me throughout the process.
