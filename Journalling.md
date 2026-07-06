# Setting Up
This is my first Hackclub project!

I've set up Hackatime, and I've been going through the (really long) Slack chats in #keeb. This is also like my first time using Github - and I'm still learning about repos, commits, pull requests and all the other stuff. 

<img width="1150" height="850" alt="Hackatime" src="https://github.com/user-attachments/assets/04e2bdb6-47d2-45be-9490-a9fc42a1ac37" />
<p> ^ - I finally set up Hackatime - and I've coded for 2 minutes so far! </p>
 <img width="1200" height="900" alt="Submission Criteria" src="https://github.com/user-attachments/assets/08730927-7500-47f6-aa70-c8d1b9298343" />
<p> ^ - I was copy pasting all the stuff to submit in my shiny new Github repo - so I don't forget to upload any of them :) </p>

I'm really excited to build this keyboard, and I hope my inexperienced design \**works**\. (I'm learning Markdown too!)

~ a-hungrybookworm

26/ 06/ 2026

# KiCad

## 3.00 p.m.

I've just installed KiCad, and installed the MarbastLib library. The Slack chat really helped with the schematic!

<img width="1653" height="497" alt="Schematic" src="https://github.com/user-attachments/assets/e76354ab-2c15-4cd3-bd9b-c576ecf59183" />

I'm placing the swithces in the matrix now.

I still don't really get how the matrix (or the code I'm going to have to write to the Raspberry Pi) works - if it checks each column and row to see which switch was pressed to connect that circuit - then how does the diode help? The current doesn't flow *over* the fourth switch if three switches on a corner are pressed together - so how does the extra node get activated? 

I guess it'll make sense after some time.

## 5.00 p.m

I'm pretty much done with my schematic now.

<img width="1333" height="921" alt="Schematic_2" src="https://github.com/user-attachments/assets/67cc8088-e21a-409b-8abb-334c49dddb52" />

So I don't have arrow keys (to save space :)), cause that space was taken up by the right shift - but I guess it should be fine, as I never use them anyway. I tried to add a rotary encoder too, but it seemed a bit complex (it had a lot of resistors in the wiring, and used a lot of pins - I'd have to change the microcontroller) and I wasn't too sure if it would work. For my first project, I think I'll stick to making it simple.

Also, is 8 stabilisers a bit too much? And the stabilisers need to be different for different sized keys - but marbastlib has only one size oif stabilisers.

I'll do the routing tomorrow.

~ a-hungrybookworm

28/06/2026

# Schematic (again!)

## 7.00 p.m.

I've been going through the chats again, and my keeb really does seem too simple. It's just a plain old boring 60% keyboard, without any cool mods. But then, I don't even know what I want to make - a corne split keyboard (like Joe Scooto)? Or do I add a rotary encoder (I feel bad about that now), or Bluetooth, or even LED lights? idk... I'll research a bit.

# PCB Design

## 7.00 p.m. 

I've been editing the sizes of the keys, and this is what I've ended up with! Each row is 14.5 units long, and each column is 5 units long. Now finally, it all fits on the Pi Pico.

<img width="1288" height="484" alt="Screenshot 2026-07-06 at 7 56 05 PM" src="https://github.com/user-attachments/assets/5b7af2c2-f65c-4d51-9b06-afbd592d2286" />

I edited the rows and columns too, so I can add the arrow keys (and the right shift), and I've removed the superfluous stabilisers - so now I have only 3! (I was getting worried about that).

<img width="1788" height="1120" alt="Screenshot 2026-07-06 at 7 50 58 PM" src="https://github.com/user-attachments/assets/67e04894-206e-4d3f-b201-e7b39d0bd110" />

The Slack chat absolutely rocks - now I'm using 19.05mm grids and that's soo much better :). And I'm going to use <a href = "https://github.com/adamws/kicad-kbplacer">this</a> plugin to place the diodes.
