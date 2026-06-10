---
title: "Helix"
author: "Arnav Gupta"
description: "My take on an Arduino"
created_at: "2026-06-02"
---

# June 4: Designed Schematic

I have been designing a development board to teach me the basics of circuit design. It will include a full RP2040, Voltage Regulator, USB-C connector crystal, memory chip, 2 rows of GPIO pins and external UART pins to be able to connect to a motor controller. My longer goal with this project is to use it as a MCU for the SO-101 robotic arm which is controlled via a UART connection. So far I have drawn up the schematic for the basic parts like memory, the USB-C connector and other miscellaneous items.

![Schematic layout](images/06-04.png)

**Total time spent: 2.5 hours**

# June 6: Finished Schematic design

I finished making my entire Schematic design. I spent quite a bit of time fixing ERC errors and arranging my schematic so it is easier to fix and change in the future. I also learned what pull up and pull down resistors are, why they are needed and how they work.

![Schematic layout](images/06-06.png)

**Total time spent: 2 hours**

# June 7: PCB Design

Today I imported the schematic into the PCB editor and i started to organize all my parts. My idea is to make it look like an ESP so it can fit onto a breadboard. This means the GPIO pins are on the sides while the RP2040 is in the middle with the Wi-Fi chip on the bottom and the USB-C receptacle at the top. During this time I was mindful to organize all the parts so when I start to route pieces together, it won't be extremely messy and easy to debug and look at.

![PCB layout](images/06-07.png)

**Total time spent: 1.5 hours**

# June 8: Route PCB

I spent time routing the main components like the ESP chip, memory, USB-C receptacle, and voltage regulator. The way I thought of organizing this was to keep as much things as I could on the front side of the PCB and then combine vias and routing on the back to connect the rest. I had to reorganize some components so the lines wouldn't be that messy and to have space for all the capacitors. One thing I made sure to keep in mind was to space the components out so I could hand solder most of them together.

![PCB layout](images/06-08.png)

**Total time spent: 2 hours**

# June 9: Route bottom layer of PCB

Today I finally finished routing my entire PCB. I used a lot of vias to connect some parts together because the paths were already blocked by the front traces, so I had to use a combination of vias, the back trace, and the front trace. I also spent a lot of time making sure that everything was connected and I didn't leave any parts behind, because this is only my second PCB ever designed and I have a lot more components. I also encountered a weird issue where the line would simply not draw coming out from the RP-2040, so I had to delete some traces for the GPIO pins around it and then start again. It kind of worked from there.

![PCB layout](images/06-09.png)

**Total time spent: 2 hours**
