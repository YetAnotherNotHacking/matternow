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

End product after my work today:

<img width="1308" height="1449" alt="{4E3ACFCD-5ABA-4297-B020-54F41C5E9826}" src="https://github.com/user-attachments/assets/94e43737-79d4-4033-89c9-fd6548879ce0" />


** Total time spent: 2.9 hour **

# May 6: Toolhead and extruder design
I worked on the toolhead geometry and figured out how I need to fit the hotend and partend fans in. I will have more time tommorow to be able to properly cool the heatsink as well. I am going to use 24v 4010 fans (2 of them) for the partend, and another one for cooling the heatsink once I get that side of the toolhead modeled up.

Fan:
https://store.dremc.com.au/en-us/products/4010-axial-fan-24v-by-dremc?variant=43214340063401

<img width="1316" height="1026" alt="{7CDF38D6-E4DA-4E34-84E7-98FFC61D22CB}" src="https://github.com/user-attachments/assets/7a295c90-f143-4cfb-8c73-593d8d0bd30b" />

the intention is for the 10 mm fans to stick out a bit, they will go in the 5 mm cavities on each side. the hotend will of course go in the middle and be fixed to the currently extruded part (the top of the sketch there). the air will enter, and then be pushed down. I may make a bit of a better guide system for the air, as its just relying on the pressure to leave how I want it to. I am actually quite happy with this design, and am excited to work on it more in the morning. It's 1 AM and I have tests tommorow so that is going to be it for today.
Here is an image of the sketch of the toolhead I have for now.

I have finished the hotend. The hotend, hotend fan and partend fans are all in place. I plan to have the wires route along the outside of the hotend, while it isn't professional, this hotend likely is not close to the final product. This is to model what it will look like. I will look into making it more rigid, that is what I will work on next.

<img width="1086" height="751" alt="{DB21C3F2-70F5-4B3E-9346-0264120B8BAD}" src="https://github.com/user-attachments/assets/e92c80c5-c999-4c19-9617-da6130f600a9" />
<img width="1052" height="887" alt="{7AF3E5E9-74E1-42BC-870A-3A904D228944}" src="https://github.com/user-attachments/assets/ee5ddb64-9c42-4c8b-8f6e-09540cee0f86" />
<img width="1139" height="836" alt="{77B06999-F015-47A3-AB30-F8F281E082A3}" src="https://github.com/user-attachments/assets/346090db-95ab-46cc-944f-754912a62abf" />

Hmmm.... thats not good:

<img width="925" height="812" alt="{6E1B2B8B-ACCA-4A2B-84D9-DF498F38FF39}" src="https://github.com/user-attachments/assets/eb13a1f2-bbe7-44e7-a974-5da83710cfad" />

I'll do the same thing that I did to fix the other gantry rails, the rail will be moved to the bottom and I will have some components go up to attack to the belt system. When doing this, I will take some of that vertical space and move the fans up. I need to stop making assumptions on height, as this just keeps happening. The aluminum extrusion will touch the build plate before the nozzle of the hotend at the moment.

I talked to the guy from our FRC team, and I am going to redo the hotend to be on the side of the extrusion. He explain the issue I would run into doing it on the bottom of the rail, and I realized he was right. The forces from the belts would very quickly just twist the hotend and it would not be printing well at all. I am going to try and design it to be mounted from the side face of that gantry compoenent.

That linear rail will now be mounted like this

<img width="1483" height="493" alt="{1907040D-1474-4672-A3ED-D421A4124846}" src="https://github.com/user-attachments/assets/b3ef674f-42c6-4187-b2c9-bcd8890acbc7" />

I spent a lot more time and have redone the bottom half of the extruder. I am measuring the top end's distance from the pullies to see how far I am going to have to make them reach now, I  have a feeling it will still be kind of far. I am worried about how much play this toolhead will have, with how far up it will be pulled on I think I am likely to run into issues with it twisting. I may raise the gantry it's mounted on in order to make it pull on the toolhead closer to the rail if nessecary (it is nessecary, im putting it off)

<img width="430" height="472" alt="{623EB091-F17E-469F-B5CE-A22039EF64E5}" src="https://github.com/user-attachments/assets/09725f19-f4cd-4f95-a795-6c9d22519f30" />

I realize that still no longer solves the problem.

<img width="699" height="641" alt="{8DCF8C42-E057-4128-B6A3-EE8720489DBB}" src="https://github.com/user-attachments/assets/4ff5527c-702f-4e90-9483-9abe1abd7675" />

im now shrinking it down further and mounting the hotend almost right up against the linear carriage. This is inspired from my friends design I took screenshots of the cross sections of above. I am using those for refferse on just roughly how this went together, and I intend to use similar blower fans like in his for my partend as well. I realize this part is more complex than I had initially though it to be.

<img width="415" height="433" alt="{50569726-E467-4705-823E-9B9EDCA2F598}" src="https://github.com/user-attachments/assets/2b537d3c-22ec-4033-b189-b02e442342c0" />
<img width="439" height="499" alt="{521DA965-AF46-43D5-B6AB-68D765141BFE}" src="https://github.com/user-attachments/assets/76ad1bcb-02b1-4b55-b09a-3413ebc79b91" />
<img width="440" height="466" alt="{72E1FAAE-737B-4AAE-854E-A01D3718C7CA}" src="https://github.com/user-attachments/assets/96e4df4a-6f45-4b77-a681-078888352d8e" />


It took some really annoying redoing of work, but it's finally there. I am really really happy with this design, I think 3 iterations made me land on something pretty good. I have a 25 mm cooling fan on the hotend, and will be integrating some blower fans at the top for the partend fan.

I used this for the step file: https://www.mcmaster.com/1939K18/
I will actually source them from: https://www.aliexpress.us/item/3256808589894042.html?utparam-url=scene%3Asearch%7Cquery_from%3A%7Cx_object_id%3A1005008776208794%7C_p_origin_prod%3A
The blowers I intend to use are: https://www.filastruder.com/products/delta-bfb0524hh-blower-fan?variant=39503824650311&_gsid=G6XowAwBG8xu
** Total time spent: 4.4 hour **
