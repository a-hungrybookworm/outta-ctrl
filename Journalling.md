# Writing Firmware

## Total time spent: 2 hours

I've used RMK firmware, and I wrote it using GitHub actions (I don't know how to code in Rust!). It was pretty easy, as I kept the extra functions to a minimum.

~a-hungrybookworm

04/09/2026

# Finishing the 3D Design

## Total time spent : 10 hours

I *did* spend a lot of time on this, but it's my first time using Onshape, or 3D designing anything much.

I'm using a sandwich mount, with a top part, plate and case all screwed together, and the plate screwed to the PCB. It might turn out a little stiff, but I don't really mind, as this mounting style was easy to design and will use less screws altogether >_<. 

I'm using 8 M3s with heat set inserts, and 4 M4s for the plate to PCB. The plate to PCB screws aren't necessary, but I'm scared that the PCB will rattle in the case, or that the switches will wobble, so I put the holes in there just in case.

For the top of the plate, I downloaded a dxf drawing from Keyboard Layout Editor NG, where I designed my keyboard. It included the holes for stabilisers too, and that was really helpful. 

I also had to split the case, as it was more than 300mm wide, so I designed a tongue-and-groove joint between the parts. For the plate, which was too thin, I put a sliding-groove-thingy - I'm not really sure if it has a specific name.

<img width="1489" height="626" alt="3D model" src="https://github.com/user-attachments/assets/23947c4f-83f6-48d5-a634-9b7622ef806d" />

^ I couldn't find models for the longer keycaps, or the stabilisers, but their measurements are included in the design, so hopefully it's okay.

Firmware!

~a-hungrybookworm

24/08/2026

# 3D Model

## 12.00 p.m.

I figured out my PCB doesn't have 3D models for the switches and stabilisers! I'm seraching them up now on GrabCAD...

## 1.30 p.m.

I'm finally done with adding the switches. The marbastlib footprint disappeared, so I couldn't update it, and I had to manually add the Cherry MX 3D model I found to each switch. ;(

<img width="1076" height="416" alt="Screenshot 2026-08-15 at 4 32 08 PM" src="https://github.com/user-attachments/assets/c79a7895-b321-4e7d-879f-9ef8f757bc20" />

After a lot of rotating the switch and moving it in each axis, the PCB looks like this... Adding the keycaps and stabs now.

## 2.30 p.m.

I couldn't rly find long keycaps, so I've put the short ones for now.

<img width="1017" height="386" alt="Screenshot 2026-08-15 at 4 46 26 PM" src="https://github.com/user-attachments/assets/c1517099-20e7-46ea-a8f9-8d37aa9bbc77" />

Anyway I'll start the 3D design.

~ a-hungrybookworm

15/08/2026

# Routing

## 11.00 a.m.

Beginning the routing!

## 12.30 p.m.

I'm finally done! I've routed the columns on the front copper layer, and the diode connections & rows on the bottom copper layer. There was a bit of trouble with the DRC, but I finally got the 53 initial errors down to 1 warning, by adjusting the settings for an 'Exposed Copper Keep Out' area, and just moving the components around. I haven't added any ground pours, as it seems a bit unnecessary, and I don't even have a GND net. I've added mounting holes though, and my Pico USB port will hang off the PCB.

 <img width="1219" height="444" alt="Routed" src="https://github.com/user-attachments/assets/b0076d37-0862-4ace-8045-c0773ef839b3" />

I generated the gerbers and drill files, and now I've added them to the repo.

All set for the 3D design!

~a-hungrybookworm

24/07/2026

# Final Touches 

## 5.30 p.m.

I designed the keycap covers and *another* keyboard layout, with less switches on the bottom row cause I don't even think they're needed.

<img width="3066" height="954" alt="keyboard-layout6" src="https://github.com/user-attachments/assets/be817736-899a-412f-b7db-6ff0d0ee0539" />

## 6.00 p.m.
Updated schematic and pcb layout.

<img width="1292" height="706" alt="Schematic_idk" src="https://github.com/user-attachments/assets/95da6ae8-050a-4e0c-8f9e-c86b718c7220" />

<img width="1857" height="601" alt="PCB" src="https://github.com/user-attachments/assets/18a80013-7b9f-48f3-9387-d6ea8e479def" />

~ a-hungrybookworm

23/07/2026

# Back to the Schematic

## 7.00 p.m

Hopefully this is the last PCB entry :)

The schematic is now fully edited for easy routing! I had to juggle the switches and diodes along the rows and columns, but it now looks like this - 

<img width="1250" height="622" alt="Schematic_last" src="https://github.com/user-attachments/assets/24ded6d7-3b98-430b-9d62-03dcf89b57ae" />

I've made the PCB using a custom grid of (2.38u x 2.38u), that is, 1/8 of a unit in millimetre (19.05mm). After a lot of dragging stuff and aligning it, it looks like this - 

 <img width="1889" height="587" alt="PCB" src="https://github.com/user-attachments/assets/5021acbe-0c32-4f3f-9bf3-9fda3bf17ae2" />

 \# Ready for routing!

~a-hungrybookworm

20/07/2026

# PCB Design

## 7.00 p.m. 

I've been editing the sizes of the keys, and this is what I've ended up with! All the keys are indented now, so I don't have to type on keys arranged in weird straight columns. Each row is 14.5u long, and each column is 5u long. Finally, it all fits on the Pi Pico.

<img width="1288" height="484" alt="Schematic_Drawing" src="https://github.com/user-attachments/assets/5b7af2c2-f65c-4d51-9b06-afbd592d2286" />

I edited the rows and columns too, so I can add the arrow keys (and the right shift), and I've removed the superfluous stabilisers - so now I have only 3!

<img width="1788" height="1120" alt="Schematic_3" src="https://github.com/user-attachments/assets/67e04894-206e-4d3f-b201-e7b39d0bd110" />

The Slack chat absolutely rocks - now I'm using 2.38125mm x 4.7625mm grids (basically 19.05 divided by 8 and 4 respectively) and that's soo much better :). 

~ a-hungrybookworm

04/07/2026

# KiCad

## 5.00 p.m

I'm pretty much done with my schematic now. It doesn't have arrow keys - to save space, but other than that it seems pretty fine.

<img width="1333" height="921" alt="Schematic_2" src="https://github.com/user-attachments/assets/67cc8088-e21a-409b-8abb-334c49dddb52" />

I'll do the routing tomorrow.

## 3.00 p.m.

I've just installed KiCad, and installed the MarbastLib library. The Slack chat really helped with the schematic!

<img width="1653" height="497" alt="Schematic" src="https://github.com/user-attachments/assets/e76354ab-2c15-4cd3-bd9b-c576ecf59183" />

I'm placing the swithces in the matrix now.

~ a-hungrybookworm

28/06/2026


# Setting Up
This is my first Hackclub project!

I've set up Hackatime, and I've been going through the (really long) Slack chats in #keeb. This is also like my first time using Github - and I'm still learning about repos, commits, pull requests and all the other stuff. 

I'm really excited to build this keyboard, and I hope my inexperienced design \**works**\. (I'm learning Markdown too!)

~ a-hungrybookworm

26/ 06/ 2026

