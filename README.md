# Keyboard Build Log
 
This document outlines my process for designing and building my first custom mechanical keyboard from scratch, including PCB design, custom keycap design, and case engineering.
 
## Journal 1: Initial Concept
**Time: 1 hour 30 minutes** 
I decided to design a 65% keyboard with circular keycaps. My goal was to create a sleek design with resin keycaps and LEDs mounted behind the switches to provide underglow lighting.

## Journal 2: Layout Design
**Time: 2 hours**
 
I began designing the schematic in KiCAD but encountered difficulties visualizing where the keys should be positioned and determining appropriate key sizes. I discovered keyboard-layout-editor.com, which allowed me to create an accurate layout template before proceeding with the actual PCB design. This tool significantly improved my understanding of the final layout.
<img width="998" height="281" alt="image3" src="https://github.com/user-attachments/assets/c1b0dad7-b9ca-48aa-afb7-6bdd20a3e6bc" />
 
## Journal 3: Schematic Development
**Time: 1 hour 30 minutes**
 
I realized that the schematic does not need to be a perfectly accurate representation of the physical PCB layout. It only needs to show all electrical connections accurately. Once I understood this principle, I was able to progress more effectively with the wiring design.
 <img width="1146" height="342" alt="image12" src="https://github.com/user-attachments/assets/9deef0b2-aa1d-487d-a270-c9579012f68b" />
## Journal 4: Switch Matrix Wiring
**Time: 2 hours**
 
I completed the wiring of all switches in a matrix configuration. I have not yet connected this to the Pi Pico microcontroller. I also need to research and integrate the two rotary encoders into the design. This step required significant research, and I learned a great deal about how keyboard matrix scanning works.
<img width="1184" height="485" alt="image8" src="https://github.com/user-attachments/assets/b363c84b-902e-4892-8ff3-4e62fa253e53" />

## Journal 5: Complete Schematic
**Time: 1 hour 30 minutes**
 
I finished wiring the complete schematic, including both rotary encoders. I added six stabilizers total, with two additional stabilizers included as spares in case they are needed during final assembly. The schematic is now complete and ready for PCB layout design.
 <img width="956" height="421" alt="image9" src="https://github.com/user-attachments/assets/569a968e-6f57-453f-81cc-c1fda0a461c4" />

## Journal 6: PCB Component Placement
**Time: 3 hours**
 
I placed all switches, the Pi Pico microcontroller, stabilizers, and rotary encoders on the PCB. I adjusted the spacing between switches multiple times to match my original design specifications. The next phase will involve routing all electrical traces.
 <img width="960" height="374" alt="image1" src="https://github.com/user-attachments/assets/7681986f-a769-4411-b3df-58c10b199c19" />

## Journal 7: Trace Routing and Verification
**Time: 4 hours**
 
This was the most time-consuming phase of the project. I routed all traces and performed verification using KiCAD's DRC (Design Rule Check) checker. I had to ensure that no traces crossed and that all components maintained proper spacing. The design has been verified and is ready for manufacturing.
<img width="1236" height="472" alt="image5" src="https://github.com/user-attachments/assets/16cf1724-c0e1-4138-b8a6-d9423e491a4e" />

## Journal 8: Custom Silkscreen Design
**Time: 2 hours**
 
I added personalization to the PCB by designing a custom silkscreen on the front with my name and a full board design on the back. I discovered that silkscreen designs must be rendered in black for KiCAD to display them correctly on screen.
 <img width="619" height="252" alt="image6" src="https://github.com/user-attachments/assets/4f5123a8-513e-474d-8ec2-4004e6a9ff3b" />

## Journal 9: Three-Dimensional Assembly
**Time: 2 hours 30 minutes**
 
I imported the PCB STEP file into Fusion 360 and began adding three-dimensional models of the switches and rotary encoders. The diodes and Pi Pico were already included in the STEP file because they had 3D models linked to their KiCAD footprints. Although manually placing each switch in its correct position was tedious, this process allowed me to visualize the final assembly.
 <img width="1124" height="368" alt="image11" src="https://github.com/user-attachments/assets/6398b5b1-28e0-45f7-99a8-4dd32b05b357" />

## Journal 10: Plate Design
**Time: 1 hour**
 
I designed the plate using Fusion's 3D sketch feature to trace the keycap outlines. This approach proved to be effective and more straightforward than anticipated. I selected a bottom-mounted configuration for this keyboard design.
 <img width="1125" height="390" alt="image4" src="https://github.com/user-attachments/assets/726e7d75-0e0a-40b1-8dd0-733bc37046f3" />

## Journal 11: Custom Keycap Design
**Time: 2 hours 30 minutes**
 
I completed the design of all custom keycaps using a circular profile with a loft feature. The longer keycaps, such as the shift and spacebar keys, presented challenges because the 3D sketch feature does not permit vertical movement of sketches. I had to redesign these sketches multiple times before achieving the desired result. I selected resin as the material for its translucent properties.
 <img width="1068" height="430" alt="image2" src="https://github.com/user-attachments/assets/333a713e-c95a-4d49-b00d-3583e2f80dbe" />

## Journal 12: Outer Case Design
**Time: 1 hour 30 minutes**
 
I designed the outer case with two separate pieces that sandwich the plate assembly in the middle, ensuring secure assembly. I selected wood as the case material because I plan to machine the case from wood stock that I currently have available.
 <img width="1068" height="430" alt="image10" src="https://github.com/user-attachments/assets/475404e7-f309-4f68-a9d4-500670bc85e3" />

## Final Render
 
I utilized my complimentary Autodesk Education cloud rendering credits to create a final visualization of the complete keyboard assembly.
<img width="1475" height="706" alt="image7 (1)" src="https://github.com/user-attachments/assets/d0498db6-207c-426a-accb-b7d5a0fc5549" />


## Total Hours

In total, I spent 25 Hours and 30 Minutes on this projects design phase. As this was my first time making a PCB, I had a big learning curve with Kicad, so it took a bit longer than expected. Helpful tools such as the Marbastlib in Kicad and 3D Sketch in Fusion helped a lot with saving time. I am excited to get my grant and order the PCB and parts!
