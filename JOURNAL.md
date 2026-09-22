---
title: "Open thermostat"
author: "Vishruth S"
description: "A small controller for air conditioners in home assistant"
created_at: "2026-09-10"
---

# September 10: Designed the product
In canva i experimented with different screen layouts, colour choices and designs before finally landing on a design that had a main wall controller similar to the actron air neo.
I made 2 designs one for the large multifunction controller likely to be mounted to a wall and the small remote, the remote can change between devices such as hvac, space heater fan or mini split and works off of espnow from the wall controller. This connects to the central hub powered by espnow and plugged in for maximum battery life. I went through many iterations of the screen layout and buttons layout and colour themes and eventually landed on what is in my opinion the best looking version with the black backgrounds, black and white oled displays for cost savings and simple buttons which may be touch capacitive later.

I designed everything in canva white baord using simple shapes. this is what is now the basis for the design and it is what the final result will hopefully look like. I hope i can make them thin enough where they dont feel super heavy or thick.

<img width="633" height="652" alt="Screenshot 2026-09-10 at 7 04 47 PM" src="https://github.com/user-attachments/assets/47dc71b7-654e-4c35-b232-bc52f5b1d84d" />

**Total time spent: 3.5 hours**

# September 12: Research
I researched on what components to use, for the small remote i decided on using simple buttons because trying to use capacitive buttons in the middle of the night would not be super pleasant and they do not offer any real benefits anyway. I chose to do the same with the larger room controller and opted to use a 2.4" monochrome OLED with normal push button switches for a more tactile feel. The displays can be purchased cheaply from Aliexpress and offer all of the functionality needed for the project such as showing temperature, being bright, having adjustable temperatures and most importantly having a low load on the esp32 for maximum power efficiency as these are both battery powered devices, with the option of a dock for charging. For the dock, i was planning on having a simple barebones style and thick heavy style of dock for the remote and having a magnetic dock for the larger main node, the magnets embedded in the back of the enclosure would adhere to a base station stand similar to that of one that the Actron Air Neo zone controller uses. The device will use a PCB to maintain a compact form factor and a Single-Cell 3.7V LiPo Pouch which is about 5mm thick to maintain a thin feel while also providing excellent battery life.

<img width="455" height="462" alt="Screenshot 2026-09-13 at 11 42 46 PM" src="https://github.com/user-attachments/assets/e20ea4b8-c25f-4db2-9d50-8b7a82863db5" />
<img width="578" height="478" alt="Screenshot 2026-09-13 at 11 42 32 PM" src="https://github.com/user-attachments/assets/1bfd492e-446c-4a97-8b5e-b25cc5a5c042" />

**Total time spent: 4.5 hours**

# September 14: PCB design
I started with the PCB design on Kicad, already having designed a macropad i had some sense of what to do, The first step was relatively straightforward i would add my 3 buttons, the screen and the board to my schematic an connect up all the wires. The first problem started when i tried to assign footprints to the symbols. When i tried to search for a 4 pin oled I2C display i incurred a serious hurdle as there was none that existed that fit what i was using. Instead i downloaded the KiCAD Mod File and imported it into KiCAD and then i had the display. After adding everything to the schematic i assigned all of the footprints and then moved to the pcb design workspace where i 
built the PCB I routed my traces correctly and used Via's to bring up the back copper face lines to the front. I added a battery conenctor for high power and long battery life when connected to a Lipo battery and easy charging capability when inserted into the dock. The PCB is one of my most complicated PCB's i have designed so far requiring SMD buttons and boards.

<img width="369" height="639" alt="Screenshot 2026-09-15 at 11 22 10 AM" src="https://github.com/user-attachments/assets/09c748af-bae2-4a23-bf53-699db20cd329" />
<img width="407" height="407" alt="Screenshot 2026-09-15 at 11 22 27 AM" src="https://github.com/user-attachments/assets/1592e685-b0be-477c-b31a-2be3a2a53378" />

**Total time spent: 6 hours**

# September 17: CAD design
I ran into multiple issues with the CAD. When exporting from Kicad i had to manually edit the footprints to include the 3d models and edit the footprints. After that it was very simple. I inserted the PCB into fusion and designed a case to ecase the PCB. I designed it very simple and to be easily rechargeable. all you have to do is remove the pcb every 2-3 months or print the version with a built in charging port. The cad process was extremely simple until i got to the lid. I designed the lid to be held in place with screws and to have only 2 visible buttons the top button would be a rocker switch while the bottom would be a single button for mode cycling and power. figuring out the rocker switch was relatively was relatively easy and only took about 20 minutes to implement. 

<img width="660" height="652" alt="Screenshot 2026-09-16 at 10 43 17 AM" src="https://github.com/user-attachments/assets/a3bdaa95-c717-49cc-96c1-12513dd46691" />

**Total time spent: 3.5 hours**

# September 22: Mounting pegs and small fixes
I added 2 things to this revision, I Added the mounting pegs for the PCB so that the board sits stable when the buttons are being pressed and when the remote is being held, it also offers a solid platform for the device. The mounting pegs were simple i created a sketch on the PCB base and extruded through as a solid object and made the pillars around it. The second fix was reducing the height of the baseplate so that the seeed ESP32 C6 would fit nicely. There wasn't much to this revision it was mostly just bugfixing and updating the design, all of the new cad files have been uploaded as well as the new render of the device in an interesting colour selection inspired by the craighill scissors which i saw on YT shorts.

<img width="628" height="280" alt="Screenshot 2026-09-22 at 2 51 53 PM" src="https://github.com/user-attachments/assets/d1d93617-61af-400f-a8cc-92876cd9f7ed" />
<img width="461" height="357" alt="Screenshot 2026-09-22 at 2 51 38 PM" src="https://github.com/user-attachments/assets/aba8d12c-9b87-49b3-90a2-bd47d11b0164" />

**Total time spent: 2 hours**
