# May 22th, 2026: Keyboard PCB + Screen Ordered

I finally got around to learning KiCad... 

I started out with looking at https://youtu.be/8WXpGTIbxlQ?si=HWInNqnCrlnGG9be to learn how to use KiCad to make the keyboard

I finished my layout for the switches. Time to start working on the wireless aspect of the keyboard!
The final idea is to have the keyboard be removable from the main body so that I can store RJ45 (Ethernet) cables and whatnot inside, so BT/wireless will be needed

The requirement of wireless pushed me to the ESP32 as it has built in BT. I already have some lying around too which is nice.

To figure out the battery, I looked at https://youtu.be/POPvclRAKOQ?si=WiUL5QYuJIJgOxCi and https://docs.google.com/viewerng/viewer?url=https://hacksterio.s3.amazonaws.com/uploads/attachments/1512547/schema_kicad_tj8aQFMW23.pdf
The video was to figure out the recharging aspect of the keyboard, the second was to figure out how to actually get power from the battery.


Today's Schematic and PCB Layout:
<img width="1093" height="824" alt="2026-05-22--22:12:51" src="https://github.com/user-attachments/assets/f3b5b7a0-08f0-4187-8efd-a98d73aac196" />

<img width="1303" height="918" alt="2026-05-22--22:12:41" src="https://github.com/user-attachments/assets/c1b02f9b-5ccc-47fd-af69-9854a74d9ef0" />

Still need to figure out my key layout and to confirm that my battery routing makes sense.

I also ordered my screens from PiHut, arriving Wednesday. (5/27/26)

**Total time spent: 4h**



# May 25th, 2026: Keyboard PCB + Screen Ordered

I forgot to complete this journal the last two days, so this update is from the 23rd to the 25th

I updated my fill zones for power to be larger since that's better for power transfer apparently. I made my top layer fully VOUT (battery power) and my bottom layer GND  for that reason. My other zones might need to be updated but from what I see they're fine for now.

Images of power fill zones: 
<img width="452" height="871" alt="2026-05-25--20:31:05" src="https://github.com/user-attachments/assets/b5273c38-a0bf-4984-92e1-fc3b06b9e400" />

I also finished my layout and routing for the keys. I decided on an ortholinear layout since I want it to be as small as possible. I think there's optimizations that I can do to reduce the size of the keyboard but that's a problem for later.

<img width="1344" height="665" alt="2026-05-25--20:26:37" src="https://github.com/user-attachments/assets/ff2ee7d5-5796-4973-a32d-d990626afeeb" />

Todo: 
1. Fix all the DRC issues that popped up
2. Figure out where to place my delete key

**Total time spent: 3h**
