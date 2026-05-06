---
title: "MatterNow 3D Printer"
author: "YetAnotherNotHacking"
description: "Yet another CoreXY 3D printer"
created_at: "2026-05-03"
---

## May 3: Initial ideas

Today I was really just figuring out what it is I wanted to do. I decided on a corexy 3d printer, figured out some of the rough hardware I will need and started putting together a basic frame for me to work more with tommorow and onward. An image is attached of the base, I need to figure out how I am going to set up my gantry so I didnt put the top corners on as that is where the motors are going to go. The base is 4 2 ft peices of aluminum [https://www.mcmaster.com/47065T101/](here) and the vertical is the same just the 3 ft option. This should be roughly perfect dimension for what I need.

<img width="500" height="auto" alt="{705EB736-B809-407A-B1C5-5BE22C0F116D}" src="https://github.com/user-attachments/assets/02b51bae-2e2a-4365-bd8b-697801a8f831" />

** Total time spent: 1.3 hours**

## May 4: Working on the gantry

Today I am working on the gantry. I have found the pulleys for drive and passive belt movement that I want to use. https://www.mcmaster.com/3684N11/ for the drive (also available https://kb-3d.com/store/motion/214-gates-powergrip-2gt-pulley-16-tooth-5mm-6mm-1634481998632.html) and https://www.mcmaster.com/3693N11/ for passive (also also available here https://kb-3d.com/store/motion/216-gates-powergrip-2gt-idler-6mm-toothed-1634482229216.html)

I also have decided to put the left belt on the bottom and the right belt on the top. I am taking a little bit of inspiration from how they designed the belt system on this page (https://drmrehorst.blogspot.com/2018/08/corexy-mechanism-layout-and-belt.html).

Here is an image of the motor bracket initial draft, it has a brace on the side to try and keep it from flexing under the tension of the belt. I will talk to a mentor from my FRC team to figure out the correct way to do it, but that's what I have for now.

<img width="200" height="auto" alt="{FB9906E1-2987-41E8-B0CE-2A526DED208E}" src="https://github.com/user-attachments/assets/99b1d635-c656-4bf8-96f0-f34aecbc722d" />

After putting the belts on, I have found the position (above the backet height, the same bracket height will be used so this measurement is fine) for each of the pulleys. The left motor driven belt will be 0.145 inches to the bottom of the belt and the right motor driven belt will be 0.385 inches above the bottom of the belt. The belt is ~0.236 inches making the distance between the belts being a tight 0.004 inches, however, I can most likely increase that if needed. I know from experience from FRC that belts rubbing together very occasionally isn't the end of the world so I won't act like it is.

I talked to one of the people from my FRC team and it turns out they have a fully modeled corexy printer they never got the funding to build, ill be using this for some design inspiration as they have a full belt path and mounting setup, but they are using 1.5 inch exstrusion while my design uses 1 inch.

I did find out that the team has an absurd amount of 1.5 inch extrusion we have no use for, BD Medical that donates our lexan also donates the extrusion from their old assembly line machines. This means if I am willing to use 1.5 inch extrusion, the cost is nothing as it's free from our shop potentially.

I will be modifying the current design to be more cost effective, it does mean probably restarting the overall machine assembly unfortunately. the current cost for all of my extrusion is a little over 165 dollars.

<img width="1233" height="1016" alt="{F5B72A12-4483-42DD-A2D2-2BB7F389D00C}" src="https://github.com/user-attachments/assets/328542f9-f090-4701-8b00-bfb2edce2f2c" />

I have finished redoing all of the parts (my intent driven sketches were horrible and didnt work so I had to completely redo them) but I did fix a few pain points of the old ones as well as take advantage of the bigger size. There are now 2 fin things for better rigidty, and its all using the "free" aluminum. (this is actually so goated, as that's about 270.24 USD worth of extrusion :P)

The beta (left) belt is about 0.146 above the top plate now (3.70mm) and the alpha (right) belt is about 0.425 inches (10.8mm) above the top plate. I increased the distance between the two belts in my redesign of the motor mount by recessing the stepper motor a bit more than previously.

I have now finished the idler pullers for the other top corners of the printer

<img width="auto" height="500" alt="{ACBB2929-7470-472A-862F-2E54F8FAF183}" src="https://github.com/user-attachments/assets/9823022f-5397-46d3-b42c-dd783b0f007c" />
<img width="auto" height="500" alt="{0ACC5BCA-425C-4C2B-9F94-D24EE917DA79}" src="https://github.com/user-attachments/assets/b0597f91-f359-494d-83f7-c4cb2d24463b" />

I have spent like half an hour looking for what linear rails to use, I landed around the area of HGR 20 Rails at about 500 mm length. This is quite large, but that is the goal with this printer (I plan to make use of it for some FRC parts in the distant future). I was first looking on McMaster and was wondering why everything was 300+ dollars just for the rail, but then I found some from an Australian store for 34 bucks per rail. (https://www.rmcomponents.com.au/products/linear-rail-hgr15-500mm-length?variant=43527262044397). I also see that they sell the relevant linear bearings (https://www.rmcomponents.com.au/products/linear-bearing-hgh20ca) so I plan to get those form them as well.


It's been widly difficult to find high quality step files of the rails that I intend to use, so I found one that sort of works that is shorter and just extruded it. I will attach it with 4 screws per rail in the real design, but, i can't model that in cad right now.

<img width="1156" height="951" alt="{E7AA2EA6-1DBF-4406-939D-C603877E7431}" src="https://github.com/user-attachments/assets/14d88a5f-86ec-48a1-bbf8-ff78ce71052d" />

I have finished putting together a rought idea of what the linear rail and extrusion for the hotend rail will look like. I have added it to the main assembly and put some sliding joints on it just to get an idea of how it will move. I will now work on the hotend and figure out how I am gonna make that work. I may take super heavy inspiration from the one the guy from my FRC team gave me, as it's very good. He did make it tool changing so I could simplify it a bit. I may also look into a way to swap it out for a higher speed extruder (my goal for thie project is 500 mm/s with 50000mm/s/s.)

Here is an image of the gantry as of now:

<img width="auto" height="500" alt="{DA1D3466-8B2F-492F-AA7D-7130686ADBC7}" src="https://github.com/user-attachments/assets/2214c62e-3340-4f67-9120-63b1e9fa3461" />

Even after lowering the secongary gantry component, I realize the rails still are raising it too high for the current heights of the belts. This will most likely be fixed by moving the rails to the under side of the top extrusions and having the printed adapter reaching back ground. I have gotten the fit pretty good with this gentry, however, I don't have an effective way to route the belts as of right now.

<img width="1377" height="304" alt="{8095E5AF-74BC-419A-B4AC-E09D0E560D44}" src="https://github.com/user-attachments/assets/1c2fc043-a875-4e1a-a092-c3d53cc7892c" />

I will have to look more into this tommorow, as it is 12:32 in the morning sadly.

<img width="2880" height="1920" alt="{98583E51-4F03-4561-92FD-94502107FA8C}" src="https://github.com/user-attachments/assets/1f436c99-551a-4e3a-b7d7-d06562dc6138" />

Ahove is a closer look at how the bracket is going to fit around the rail carriage and extrusion it is mounted on. I think just turning it all upside down should hopefully work (emphasis on hopefully, I have no idea. I am trying things as I am going on and I hardly have an idea of what I am doing in CAD on top of that.)

Overall product at the end of the day:

<img width="1081" height="1240" alt="{FDB88FC5-DADD-416F-A976-9FD24660C74C}" src="https://github.com/user-attachments/assets/c92e7369-be11-4069-a437-5a7822cafdcf" />


** Total time spent: 7.7 hours**

# May 5: Working more on gantry and starting hotend ideas

<img width="953" height="615" alt="{E8419A7E-8B5A-4533-88D1-CED35462002D}" src="https://github.com/user-attachments/assets/2d7bf96a-ec6c-46c9-94b4-37bf63cdf9c8" />

I have moved the gantry to be under the top of the printer like I mentioend that I was going to do yesterday, and that seems like it might work in this orientation. I have also checked the movement limits and I see that we can have our hotend stick out 2.9 inches from each side of the linear bearing, thats probably more than I need but that just defines the maxiumum clearance I have for any blower fans I want to add for the partend. I also tested and we are 420x420mm on the gantry, I am unsure of how big I can make the z axis with this scale so I will figure that out in the future.

<img width="1448" height="346" alt="{9F3301B8-3713-4668-850C-9C2E718D690B}" src="https://github.com/user-attachments/assets/5c3bfbb7-79f8-4262-9817-e4910b829a51" />

I now have these tabs going up over the extrusion, and I will be able to mount the pullies here just fine. This also actually simplifies where I am putting the homing switches so this is actually really good I ended up changing the design in this way.

<img width="1394" height="1340" alt="{C5ABF086-B28C-4B3D-B561-7C8FC995DD32}" src="https://github.com/user-attachments/assets/65335fa7-91a6-477f-ab33-51a7778215ea" />

I have finished modeling in the pulleys and how they will mount to the secondary linear rails on the gantry to the overall model. All thats left for the rest of this gantry is the hotend and how the belts attach to it. I already know that I am going to be using a remotely driven hotend to make the print head as light as possible. I am now doing some research to figure out what the best hotend and extrusion setup is for this kind of printer.

After quite a bit of research, I ended up choosing the Phaetus Rapido 2 UHF (which happens to be the same one in my friend's design). I assumed since he made his about 3 years ago that it wouldn't be the best and that it would be outdated, however, with the specs it has and the long melting zone I really can't find anything better than it. It is a little hefty in price, but, its hefty in specs too.

<img width="956" height="1312" alt="{449CA87A-A0C8-4148-A5F5-FC44C8D371F8}" src="https://github.com/user-attachments/assets/8e744e33-d7f4-4817-a754-afe87d9c7b68" />

I did end up finding a step file for it, and I have been drafting the layout for the toolhead. I will post an image once I get stuff actually layed out better.

I do also have some concerns about the scale of the printer. I know 420x420 is a huge build area, but after putting it on an a tape measure and putting a scale to the project I realize I might have made a little bit of a mistake. I think it will be fine, it will be better for the end goal of being able to manufacter FRC parts better, and the aluminum is free and the rails at this size are still cheap ish, but I def might want to watch my scale more in the future.

I am looking at my freind's mounting methods for a similar nozzle (apparently it wasnt a rapido, he said it was when it isn't that in the cad)

<img width="453" height="744" alt="{60ABA0D2-6653-4DD3-BC15-7946235EDC65}" src="https://github.com/user-attachments/assets/2ac62318-630a-41b0-96b8-cf09f7daad47" />
<img width="629" height="1083" alt="{AD3DCA24-75A7-4650-A810-924D56F5146D}" src="https://github.com/user-attachments/assets/e9b2127f-1460-427a-a503-44abf3e69097" />
<img width="923" height="1194" alt="{523A57BB-9B8D-466D-A3CF-094B46F8AD64}" src="https://github.com/user-attachments/assets/74ce4332-2967-458e-b751-46ae7c58dd08" />

I am going to attempt to do the same thing that he did here, I like how the hotend works. I don't want to copy the switchable head system he has, as I don't have a real need. I can swap it out still but I don't need a quick swap system. I believe he did this because he prints TPU a lot for our belts on our robot. I don't really like the cooling pathway he had too much either, I don't think there is much of a way around it though. I thing I could get the fans closer to the part but I am not sure that's going to be worth the effort. I will continue modeling the toolhead on tommorow's journal as the day has turned (its 12:26 am)
** Total time spent: 2.9 hour **

# May 6: Toolhead and extruder design
Nothing yet...

** Total time spent: 0.1 hour **
