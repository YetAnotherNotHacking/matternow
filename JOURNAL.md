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

So instead of blowers I decided to go back to using the fan I planned on using in the old design, I realized it's just the easiest at this point.

<img width="393" height="561" alt="{68D64B8D-79FE-45B3-BF9B-68E64C0013C5}" src="https://github.com/user-attachments/assets/5edfa68c-e737-4191-98e4-dce12cf8ce27" />
<img width="451" height="554" alt="{EEA8DCFA-E45A-4F62-8CAD-AE36B54E9BE8}" src="https://github.com/user-attachments/assets/9a2d25b0-8a2e-4611-9550-49f6875a1e9d" />
<img width="457" height="642" alt="{0F7E1324-0145-40FD-A2A4-5C65CFC43530}" src="https://github.com/user-attachments/assets/b54abf82-d15f-4b28-85a3-9f3de8f8dd83" />

I am going to add this issue to the main assembly and see if there are any glaring issues again, if not, I will get the belt connection points put into it. Part of the motivation for putting the fans up so high is that is around where the belts are going to have to connect, so having stuff there makes it like more effecient or something idk.

<img width="569" height="678" alt="{F3266182-F30E-4C9E-BC8D-DC9F6FF7466D}" src="https://github.com/user-attachments/assets/c4b806d0-6b4e-4b2d-9390-9a73a745f53d" />
It looks pretty good IMO! I will extrude the top bit up enough that its level with the other brackets, and then attach tbe belt to posts. I plan to have it rap around, where the belt forms a u and the peg goes in the cup thing of the u. It will be secured with a zip tie on the other side, its similar to what you might see on another chinese printer (very high quality yes yes)

<img width="287" height="425" alt="{F16ED97C-595A-4783-AB7B-A05423CBF89D}" src="https://github.com/user-attachments/assets/64a49b89-5c82-4567-b2ed-23722a57f611" />

I am going to have to move those pullies over for this work work, but that is the defenition of a tommorow task. I am too tired. I do want to write out a quick parts list for the aluminum to ask if I am able to use it tommorow during a robotics meeting:

| Extrusion            | Quantity |
| -------------------- | -------: |
| 1 1/2 Inch × 2 foot  |        8 |
| 1 1/2 Inch × 3 foot  |        4 |
| 1 1/2 Inch × 33 inch |        3 |

As usual, here is the finished product after my work today:

<img width="646" height="759" alt="{A5736B52-B69C-4669-AEE0-C61068FBB57E}" src="https://github.com/user-attachments/assets/e2bd4db7-fdcf-452c-aefe-4bbc65e084cc" />

** Total time spent: 5.5 hour **

# May 7: Misc. design discussion and figuring out how I am going to fix the belts.
Today I spent a lot of time talking with people that are a lot smatter and more experienced, being both of the main adult mentors at our robotics shop. One of the mentors pointed out the printer that he had at our shop, an AnyCubic Cobra K2 Max already had a print bed almost exactly the size of what I need, my gantry is 420x420 in motion and that printer has a 430x430 bed. I am going to take advantage of this and have a heated bed in the project by using a replacement bed for the printer.

I also talked to the main mentor of the club, and found out a lot of good things. He has an idea for how I can get the toolhead to move with the weird belt layout, and it involves putting a plate between the carriage and the toolhead that reaches up. This would be made out of a strong and light material (not pla, most likely metal) and connect up to the belts. He also pointed out an issue with my belts, being how small 6 mm gt2 is. He helped me understand in context looking at other printers, and explaining why they use the belts that they do, and that with a gentry as chunky as mine that I am most likely not going to be able to move it fast (most likely at all) with the motors and belt that I have on there. He also pointed out the issue with using a 1.5 inch extrusion on the secondary gantry, and I realize he is very right. I am going to look into using a smaller lighter gantry, I somehow didn't concider the weight of that gantry when trying to figure out how to make the toolhead move as fast as possible. So essentially, I am going to have to use bigger (wider, probably 9mm) belts, make that part of the gantry a lot lighter, and implement some sort of plate to help the toolhead be at the correct height for the rest of the belt path.

I also did some work to start designing the lift for the build plate. I am taking inspiration from Practically Printed's earlier designs, as they seem be pretty agile and not too complex for the scale I am trying to implement them at.

For this, I am using a second version of the t bracket base from yesterday/the day before I can't remember but with a place to mount a stepper motor. The plan is to have a rail and screw with this as well, with the load being supported and lifted by the crew and the rail keeping it in line. I might have to use some custom alumimum or something to get it to attach to this AnyCubic bed, but I will be crossing that bed when I come to it.

<img width="619" height="574" alt="{3FDA30AE-A30D-465E-A3F5-995E072BBF91}" src="https://github.com/user-attachments/assets/c0e5e04a-4d96-4dd2-994b-677823c3e83c" />


The time does include a little bit of the time I spent talking to the mentors and the time I spent taking notes on how I would have to change the design. I did spend a lot of time trying to find couplers and z scews and was not able to find many of them.

** Total time: 1 hour **

# May 8: Working on z actuator for the bed
I am currently in LV for Jackpot, and spent a lot of time exploring the strip today rather than working on this project. I did get a little bit of work done waiting in the airport but I couldn't plug in a mouse and my trackpad was irritating me. 

<img width="400" height="369" alt="{8543E6F4-3E8F-4661-BC3E-CBB0D7D71536}" src="https://github.com/user-attachments/assets/27c31de1-c211-4f0f-91a2-5625af1828e8" />

At this angle, you are able to see that the motor for the z motion goes past the bottom of the printer. This will cause it not to sit flat, so I am going to simply move it up a little further.

<img width="436" height="488" alt="{86F218C1-7409-4582-B6DD-6A6F59D75389}" src="https://github.com/user-attachments/assets/7f1a6a42-9b7c-4c7c-af05-7eb592c3753c" />

When I attempted to edit it, the entire timeline broke, so I just redid it. Above is what the new design looks like.

I have finished a initial design for the linear actuator

<img width="357" height="559" alt="{A5C22610-848F-4D58-8FF0-C27639F19C79}" src="https://github.com/user-attachments/assets/6ff7114c-7c1c-4fdb-88e3-997377f62aa8" />

<img width="512" height="452" alt="{1DCD411F-9398-4E8C-A637-88305EDCFB9D}" src="https://github.com/user-attachments/assets/d8c96a0a-f006-41c4-b4c5-c869ab8b505f" />

It uses Golbilda lead screws (def not biased from ftc, they are actually cheap)

I am going to go to sleep after I put these into the main file, as I need it for Jackpot tommorow :D

It just barely doesnt hit the bar on the limit of the movement, I am so proud of that (leave out the fact that was an accident)

<img width="569" height="448" alt="{EA1B861D-E8AA-4BDD-AE45-8FA78D76FC30}" src="https://github.com/user-attachments/assets/617ed435-0cd2-4323-966c-9f7c5dbf9cc1" />
<img width="390" height="738" alt="{FEBBFD93-C846-4BAB-A354-41D80EFA0F4D}" src="https://github.com/user-attachments/assets/c45d9606-42bb-4405-8b85-1b0a6c3a101f" />

This is what I am going to use to know how far I need to have the bed above the bracket, it shouldn't be too far.
<img width="538" height="488" alt="{9C9B85DF-9DA2-45DD-9A6A-AC777790285E}" src="https://github.com/user-attachments/assets/3ea27592-4031-43e7-8a51-708ab3dd416b" />


** Total time: 0.6 hours **

