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



# May 25th, 2026: Almost done with keyboard layout!

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

# June 3rd, 2026: Done with keyboard layout (hopefully)

I finally got around to finishing the keyboard (why does school exist?)

I swapped out my esp32-D to the esp32-S3-mini since I saw that it was better for keyboards. I also ran DRC and fixed all the issues that popped up

I also gave up having a delete key, my reasoning was to just go the macbook route and bind Fn+Backspace to be delete.


Finished keyboard: !!!
<img width="1394" height="621" alt="2026-06-03--17:48:57" src="https://github.com/user-attachments/assets/47f82b9f-2dab-4da6-93f8-139b3c5eee78" />

**Total Time spent: 3h**

# June 13th, 2026: Starting on cyberdeck body

We got our slides, got our screen, and so we can start working on the body of the actual deck! 

I started with this inital design for the front back piece: 
<img width="1463" height="844" alt="image" src="https://github.com/user-attachments/assets/dcfbc506-abdd-491f-aa0a-72338d362411" />

I 3d printed it out and I found that it was lacking in sizing, it was way too large to really fit any common box form factor. I also found that it would look super weird since I would have like 2.75 inches of bezel at the bottom... (yikes!)

I thus redesigned to 1) have my casing dimensions in mind when designing and to also 2) have the bezel and appearance in mind as well.

Case: https://www.amazon.com/HUL-Professional-Cosmetic-Storage-Organizer/dp/B0827NJYD8?crid=TFEA84E0KTJJ&dib=eyJ2IjoiMSJ9.rezswYNdOSCG4tvUGmV9THGGqj9KwbnlFh8JHkMdXXG_HBH_3PKOIiKCYXN25ncSaDlXAxxLfNM_vgZEuf_T-v0boXSunR4jvgFn7yRBBjeII85gzR19NqYnbnMHKiMMYzD54RaE-Eh5f0X8hKqalnKlCWZyKu4fVrwLMu0KxEh7S2sQMBUokrwRBAsoj8oHpT7cMTG2wajvNCv51wMBGX7T0xK30CXujbunYfgzJ9Y.Sq_qqtQDbFK2J7h-ktjYJibOdYvuLneK4R34tsnplCU&dib_tag=se&keywords=hard+case+box+10+x9&qid=1781391413&sprefix=hard+case+box+10+x9%2Caps%2C186&sr=8-4 

(I didn't really want to go with the pure 3d print case as to me that doesn't really feel "cyberdecky")

Redesign back panel v2:
<img width="918" height="723" alt="image" src="https://github.com/user-attachments/assets/2fdb3598-d2a1-4229-9325-07e2a51a8f11" />

PCB update:
I was using my other laptop to design my pcb keyboard, and I was an freaking idiot as I didn't make any backups on my ssd for the pcb and I also didn't upload to github my gerbers AND I switched distros to arch from nixos since I couldn't install tooling on nixos because of packaging issues. TLDR; I LOST ALL OF MY PCB FILES :D

**Total Time spent: 2h**



