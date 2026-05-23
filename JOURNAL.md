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

**Total time spent: 4h**
