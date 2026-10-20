# L8 - Design Something Useful

# Reading

Designers must ask smart questions throughout the design process to help clarify what the issue is and possible ways of fixing it. There are two different types of questions a designer can ask: Open-ended questions and closed questions. Open-ended questions are questions that help designers explore and clarify what is going on where closed questions are typical yes or no questions. A good question doesn't depend on the type of question where it focuses more on empowering creativity, challenging assumptions, encourage reflection, and often lead to breakthroughs. Good questions will find the root of the problem, challenge assumptions, and give a better understanding of context. There are many methods to asking questions, but one big is the 5 whys. This method has the designer ask why to a general statement 5 times. When you ask why 5 times, the theory is that you should have found the root issue after those5 questions.

# Problem Statement

The first idea that I had was some type of display area. I was thinking of creating a platform with a cutout of a circle. I will then place a separate circular piece in that cutout so that it will spin - displaying whatever you want to put on the platform. I didn't really like this idea though, so I started to think about stuff that is happening to me currently. I have become incredibly sick over the weekend, and I wish I had somewhere to put all of my miscellaneous stuff and medicine. I didn't really have anywhere to put it, so I think this will be a useful product I can use and other people going through a similar situation can use.

When I started to think of solutions for this problem, I thought of the same spinning platform. I can put a rod in the middle of the rotating disc, and spin the platform using this rod. This will allow me to store whatever I want on a circular platform while being able to easily access different items in storage. I also thought it may be a good idea to put some type of stopper for the rotating disc, so it can act as just a regular platform. 

# Design

## CAD Modeling

There will be 3 different parts for my design: The base, the disc, and the pin. The base will hold the disc to spin around in while having a hole in it to stop the spinning with the pin. The disc will be able to fit inside of the base while having a tall rod in the middle of the disc. The rod in the middle will make it easy to twist the design around. There will also be a hole in the disc so I can slide the pin through the base and disc, stopping the rotation. 

I decided to model the base first, the disc second, and then the pin last. I then combined all of them in an assembly at the end to see how everything would work together.

<table style="width:100%;">
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="base_sketch.png" alt="base sketch" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        To first start designing, I wanted to know how big I should make my base for the platform. To do this, I measured the only medicine I own, an ibuprofen bottle. I measure the diameter of the ibuprofen bottle to be about 1 and a fourth inches. This means my base should have at least a radius of 1 and a fourth inch. I think I want to make it slightly bigger though, so I am going to make the radius of the platform 2 and and a half inches.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="base_extrude.png" alt="base extrude" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I didn't have an exact idea of what I wanted to extrude it to. I was thinking of creating a lip, to hold anything that may get spun to the edges, and there will be a shell in the end. With those factors in mind, I settled on 0.75 inches, which should be plenty for what I am doing.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="base_shell.png" alt="base shell" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        After, I created a shell of the base. I decided to make the shell 0.25 inches. I decided this for a few reasons: there should be less error when printing due to the bigger size, I will be able to make the disc 0.25 inches, and there will be a big enough barrier for things spun to the outside of the system.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="base_fillet.png" alt="base fillet" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I then applied a fillet to all of the sharp edges on my base. I didn't have a value in mind for the edges, it just had to be rounded. That is why I stayed with the default radius it gave me: 0.1in. 
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="disc_sketch.png" alt="disc sketch" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        To find out where I was going to put the hole for the pin on the base, I decided to make the disc to see the exact geometry I would be using so that I could better dimension my part. To start my disc, I created a sketch with a circle that has a diameter of 4.45in. Since the diameter of the base is 5.0in, and the shell is 0.25in, I am left with 4.5in of material. I chose 4.45in to give the platform a little bit of breathing room so that it can actually rotate.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="disc_extrude.png" alt="disc extrude" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I planned for my disc to be extruded by 0.25in, so I extruded it by 0.25in. 
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="disc_rod_sketch.png" alt="disc rod sketch" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        After I extruded the main part of the disc, I decided to create the rod in the middle. To make my dimensions consistent, and hopefully minimize printing errors, I decided to make the diameter of the road to be 0.25in.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="disc_rod_extrude.png" alt="disc rod extrude" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        To find the extrusion height I wanted to use, I had to make sure that it was taller than most of the products I would be putting on it. I measured the height of my ibuprofen bottle to be 2 and a fourth inches. To clear this measurement, I made the height of the rod to be 3.0in. It is a round number and should give me enough space to spin the disc to what I want to access.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="disc_fillet.png" alt="disc fillet" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        Now that all of the main features of the disc were created, I rounded all of the edges to make it nicer to look at and hopefully function better. The fillet radius is the same as the base: 0.1in.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="disc_pin_cutout_sketch.png" alt="disc pin cutout sketch style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        Now that I have the disc designed, I can start to think of where to put the holes on the disc and base for the pin to slide in. To create the sketch for the pin on the disc, I just create a circle that has a diameter of 0.2in that was in the middle of the extruded part. 
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="disc_pin_cutout_extrude.png" alt="disc pin cutout extrude" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I could make the depth of the hole a bunch of different values, but I decided to use 1.0in just because it was a round number. 
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="base_pin_cutout_sketch.png" alt="base pin cutout sketch" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        Now that I have a diameter size, and the exact location for the pin hole on the disc, I can create the hole for the base. I made the diameter of the circle 0.2in and the distance from the bottom of the base equal to the shell value plus the radius of the hole and the extra material on the bottom of the disc. This gave me a height of 0.375in.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="base_pin_cutout_extrude.png" alt="base pin cutout extrude" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        Extruding this cutout was super easy since it will go through the entire face of the base so that the pin can connect to the hole created in the disc. So I chose the "to next' option when choosing my cut value.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="pin_sketch.png" alt="pin sketch" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        My base and disc are complete now. The only thing I need to model is the pin to stop the rotation. Since the diameter of the holes were 0.2in, I decided to make the diameter of the pin to be 0.175in. This should give it enough room to fit between the holes created even if the 3D printer doesn't print the exact values. 
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="pin_extrude.png" alt="pin extrude" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        The combined length of the holes is 1.25in, so I decided to make the pin slightly longer so that it is easy to put in and take out. This is why I made the pin length 1.5in.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="final_model.png" alt="final model" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        All of my parts are completed, so I can put it all in an assembly to see how everything will fit together before committing to 3D printing. Based on my assembly, it looks like everything fits well together, and I think it should fulfill the job I want it to do.
      </div>
    </td>
  </tr>
</table>

## PrusaSlicer

I imported everything at once, and I had to flip the base and disc by 90 degrees along the x-axis in order for them to be flat on the bed. The base and disc didn't fit next to each other, so I had to set them in the corners of the printing bed. I made sure that they weren't too far in the corners where it would interfere with the initial filament process of the Pursa printer. The pin is very small compared to the base and disc, so I placed it anywhere on the plate. 

<p align="center">
  <img src="inital_layout.png" alt="initial layout" style="width:50%; height=auto"/>
</p>

To see if I needed supports, I went to the paint on supports options and clicked the "automatic painting" option. Based on the "automatic painting" option, the only object that needed supports was the disc. This is probably because the whole inside the disc is 1.0in long, which is a pretty long distance without supports. This is shown g

I kept my layer infill the same as the default: 15% infill with the grid pattern. I thought that with my simple design, the infill I chose wouldn't matter that much. That is why I kept it as default. I applied similar thinking to the rest of my settings as well. My layer thickness is 0.2mm, there was no need for a raft, and my wall thickness was 0.9mm.

<p align="center">
  <img src="infill.png" alt="infill" style="width:50%; height=auto"/>
</p>
<p align="center">
  <img src="layer_height.png" alt="layer height" style="width:50%; height=auto"/>
</p>

I decided to use PLA because I thought it would give me a smoother finish than PETG, and there was a 3D printer with a lot of PLA filament already loaded in it. The total number of layers my print will have is 418, which is a lot more than my previous prints. The total time it will take my artifact to print is 2 hours and 26 minutes.

<p align="center">
  <img src="slice_info.png" alt="slice info" style="width:50%; height=auto"/>
</p>

## 3D Printing

To start 3D printing, I exported my PrusaSlicer file as a Gcode onto a usb stick and looked for a 3D printing machine to use. I saw the machine 15 had the most filament left in it, while using PLA, so I decided to use machine 15 to 3D print my design.

<p align="center">
  <img src="machine.jpg" alt="machine" style="width:50%; height=auto"/>
</p>

The 3D printing process was going to take a while, so I decided to a few progress pictures. The picture below  shows the printing process in it's early stages. It is still printing the first layer. You can see the supports starting to form on the disc already with that little square coming off of the disc.

<p align="center">
  <img src="early_print.jpg" alt="early print" style="width:50%; height=auto"/>
</p>

I also wanted to get a video of the infill getting 3D printed, since I thought that was the most interesting process. The video below shows the print at around 50% completion. The infill is still visible, but it is starting to get covered by another solid layer as seen for the disc. The supports are also very noticeable for the disc as the entire hole is pretty much completed now.


<p align="center">
  <img src="printing_video.gif" alt="printing video" style="width:100%; height=auto"/>
</p>

The last progress update I did before letting the print finish was at 63%. This was the time in the 3D print where each part is starting to really take shape, and you can picture how everything will fit together.


<p align="center">
  <img src="print_63.jpg" alt="print 63%" style="width:50%; height=auto"/>
</p>

Here is what the final print looks like. I think the surface looks pretty smooth for being 0.2mm layer thickness and it appears that everything printed correctly. I didn't need the scraper to get my parts off the bed, since I could just pull them off by themself. It was kind of hard to get the supports removed from the hole in the disc since it was a lot tighter than I expected. To get rid of it, I started with a file and then worked my way to smaller and smaller tools until all of the supports fell out of the hole.


<p align="center">
  <img src="print_completed.jpg" alt="final print" style="width:50%; height=auto"/>
</p>

## CAD Files
If you are interested in the CAD files, here they are.
  Base: [CAD File](Base.SLDPRT)  |  [STL File](Base.STL)
  Disc: [CAD File](Disc.SLDPRT)  |  [STL File](Disc.STL)
  Pin: [CAD File](Pin.SLDPRT)  |  [STL File](Pin.STL)
  Final Design: [Assembly File](final_design.SLDASM)  |  [PrusaSlicer](final_design.3mf)


## Demonstration

Here is a demonstration of me using my design. I think it works pretty well. I am able to put multiple objects on the wheel while spinning the disc to access whatever I want. It fits what I wanted to fit on there originally, and I think I can add different things to it in the future. The pin also doesn't have as much room to move around as I thought because the hole for the base became a little deformed during the printing process.

<p align="center">
  <img src="demo.gif" alt="demo" style="width:100%; height=auto"/>
</p>

## Improvements

The main improvement that I can think about is adding some type of ball on the bottom of the disc to make it spin more smoothly. It spins pretty well currently, but I think it will spin better if it was apart of some ball bearing system somehow. I just don't have marbles that small, and I don't think 3D printing something that small will turn out well, so I wasn't able to test it.

The next improvement I was thinking about was creating a second hole on the exact opposite side of the design. I think if I had two holes, it would make the disc more secure during the none rotating moments. Currently, the disc flips up on one side when some pressure is applied, and I don't really like it.

The last improvement would be to add some type of rubber feet to the bottom of the base. To spin the disc, you kind of have to be holding the base in order for it not to twist with the disc because it is not really grounded to whatever surface it is on. I think if I add rubber feet to the base, it will become more stable and better to use. 

# Lessons Learned

I learned about different methods for creating smarter questions. I learned that slowing down the process to really understand what is going on can help accelerate production and have an overall better product. I should probably have more medicine than just ibuprofen for any situation after this because it was really hard to get all of this done while being sick. There is less noticeable error in 3D printing the bigger the parts are. My previous designs have been smaller, and I have had to do a lot of reprints for those designs because of inconsistencies in smaller measurements. With this larger design, I was able to print it on the first try with pretty good accuracy. Some of that may be from experience from past projects though.

This assignment took me about 6 and a half hours.
