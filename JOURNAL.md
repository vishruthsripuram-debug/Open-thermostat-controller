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
