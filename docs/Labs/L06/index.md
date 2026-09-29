# L06 - Design Fits for an Artifact

## Objective

The goal of lab 6 is to create a snap fit design for an artifact. The artifact was picked from a pile of leftover electronics that were given out during the lab period. There were all types of components such as motors and circuit boards. When I went up, I was left with a University of South Carolina motor circuit board. Here is what it looks like.

<p align="center">
  <img src="artifact.jpg" alt="artifact" style="width:50%; height=auto"/>
</p>

## Analyze

### Initial Design

When I was first thinking of snap fits that I could put on this circuit board, I originally thought of an electrical box (a box where you keep all of your electronics). I didn't want the board to moving around a whole bunch while in the electrical box, so I also wanted to add these little supports through the holes in the circuit board. To make this a reality, I was given a pair of calipers to measure the different dimensions of the circuit board. The important dimensions I measured were the length, width, height, location of holes, and the hole diameters. Unfortunately the hole diameters were different from each other, so I will have to be super careful when designing.

<p align="center">
  <img src="dimensions1.jpg" alt="dimensions of circuit board" style="width:50%; height=auto"/>
  <br>
  <em>Dimensions measured with calipers</em>
</p>

<p align="center">
  <img src="original_design" alt="original design" style="width:50%; height=auto"/>
  <br>
  <em>Original design</em>
</p>

### Final Design

When I was designing the electrical box, I wanted to first design the base. Since I had so many more dimensions for the supports I was putting through the holes, I thought it would've been important to get a template for this part of my design. However, through designing, I realized that this would take way longer than I expected. There was a lot of trial and error when printing just the base of the electrical box. This is why I changed my design from an electrical box to just a platform that the circuit board will snap onto. I decided to make the snap points on the supports for the holes because they took me the longest to validate the dimensions. 

<p align="center">
  <img src="final_dimensions.jpg" alt="final dimensions" style="width:50%; height=auto"/>
  <br>
  <em>Dimensions used when making the project</em>
</p>

I also had to take new dimensions from those original ones because the supports didn't line up correctly with the holes. I had to validate all of my dimensions once again, and they ended up being more accurate than previously.

<p align="center">
  <img src="final_design.jpg" alt="final design" style="width:50%; height=auto"/>
  <br>
  <em>Final design</em>
</p>

#### 3D Modeling

<table style="width:100%;">
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="base_sketch.png" alt="base" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        The first step I took in creating the base was by making a sketch for the box. I just took the length and width dimensions of my measurements, and inserted it into the box. Also, so it is not impossible to get on, I added an extra 100 thousandths of an inch. This will give my circuit board breathing room. I also noticed that one of the edges of the circuit board sticks out a little bit on the corners, so it will make up for that.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="base_extrude.png" alt="height" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        After, I extruded the base to the height of my measurement. I didn't parametrically design these first two steps because it was only one measurement and would've taken about the same amount of time to change the values either way. 
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="shell.png" alt="shell" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I then created a shell that is the same thickness as the extra dimensions I added to the base (0.1in). I know I said that I was doing it to make room for the circuit board, but my base is hollow enough to where just the wires on the bottom of the circuit board will be touching the base. The actual board will sit on top of the walls.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="variables.png" alt="variables" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        After that was completed, I could move onto dimensioning the supports for the holes of the circuit board. To do this, I created global variables for the smaller hole diameters, the distance the smaller holes are from the right wall, the bigger hole diameters, and the distance the bigger holes are from the bottom wall. 
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="hole_diameters.png" alt="diameters" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I assigned the respective diameter variables to the respective holes initially. My design did round the values to 2 significant figures, but I am pretty sure the true value is still shown if you click on the dimension. It could be cleared up in a drawing sheet.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="hole1_hor.png" alt="horizontal measuremet." style="width:100%; height:auto;">
      <img src="hole2_hor.png" alt="horizontal measuremet." style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I started by dimensioning the smaller holes first. I noticed that my measurements were taken from the edge of the holes to the wall; however, SolidWorks takes the dimension from the middle of the circle. To get around this, I added the radius of the circle of the dimension I measured, by using my global variables form earlier. I applied this technique to the horizontal distances of the smaller holes first.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="vert1.png" alt="hole1 vertical" style="width:100%; height:auto;">
      <img src="vert2.png" alt="hole2 vertical" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I then applied this technique to the vertical distances of the smaller holes. 
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="hole2_vert.png" alt="larger holes from bottom" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I did a very similar process for the larger holes. They were the same distance from the bottom wall, so I decided to line them up with the same dimensions before inputting their distances from the side walls.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="hor1.png" alt="hole1 horizontal" style="width:100%; height:auto;">
       <img src="hor2.png" alt="hole2 horizontal" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I then added their distances from the side walls using the same technique I have been using for the dimensioning of the holes.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="hor1.png" alt="hole1 horizontal" style="width:100%; height:auto;">
       <img src="hor2.png" alt="hole2 horizontal" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I then added their distances from the side walls using the same technique I have been using for the dimensioning of the holes.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="holes_extruded.png" alt="extruded holes" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        Once all of the holes were dimensioned, I extruded the entire sketch. I already had a measurement of the height of the circuit board, so I made sure to clear the height of the circuit board so that there will be enough room for the snap fits on the board.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="plane.png" alt="plane" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        To create the snap points on the design, I had to create a plane that was at the height of the circuit board. To do this, I made a plane coincident with the bottom of my design, and then displaced the plane by the height of the circuit board plus the height of the design.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="snap_sketch.png" alt="snap sketch" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I then used the newly placed plane to create a sketch around the already made supports. The diameter of the snap fits are the original diameters plus 0.02in. I chose a very small value because the fits of the supports were already pretty snug on the circuit board. If I made them too big, only half of the design would snap in.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="snap_extrusion.png" alt="snap extrusion" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I then extruded the snap fits up, since I created the sketch at what should be the absolute top of the circuit. I extruded them by 0.02in again because I thought this would enough material to hold the design in place.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="fillet.png" alt="fillet snap edges" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        Finishing the design, I rounded the edges of the snap fits to make it easier to snap on and off. I didn't want my snap fit to lock in my design forever, similar to lab 5, so I this was just an extra precaution. 
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="final_design_CAD.png" alt="final design CAD" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        Here is the final model for my design.
      </div>
    </td>
  </tr>
</table>

once I had my design fully 3D modeled, I exported the file as an STL file so that I could move onto PrusaSlicer. If you are interested in looking at my CAD file or my STL file, here are the downloads: [CAD file](final_design.SLDPRT)  |  [STL file](final_design.STL)

#### PrusaSlicer

<table style="width:100%;">
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="rotation.png" alt="rotation" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        My part came in sideways, so I had to rotate it 90 degrees along the x-axis to lay it flat on the printing bed
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="infill.png" alt="base" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I have done a lot of test prints at this point so I wanted my print to have a lower print time. To have a lower print time, I thought lowering the infill would be a good idea. I lowered it to 10% infill from the default 15%.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="layer_height.png" alt="layer height" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        To make it print faster, I decided to keep the layer height at 0.2mm. I think it will keep the design somewhat consistent while keeping a faster print time.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="skirt.png" alt="skirt" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I put a skirt on my previous prints, because the walls were much thinner, but I decided to have no skirt on this print. Also, it will increase my print time.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="final_specs.png" alt="base" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        Here is the final specifications of my design. It will take about 28 minutes to print, which is almost 10 minutes faster than my previous prints. I am also using PETG. There is no real reason behind using PETG other than that was the printer had PETG loaded into it.
      </div>
    </td>
  </tr>
</table>

I exported my file as a G-code file and went to use the 3D printers.

#### 3D Printing

For my prints, I decided to use printer 4. It was out of filament when I got there, but it was the only one open. I was able to reload it with the same material that was in it before, so I had a lot of material to play with for testing. To reload the 3D printer, I purged the previous filament while feeding the new filament through the intake. I was surprised with how much filament I had to purge even though there was nothing on the roll.

<p align="center">
  <img src="filament_refill.jpg" alt="filament refill" style="width:50%; height=auto"/>
</p>

After I refilled the 3D printer, I put the usb into the 3D printer and started my print. It will take about 15 minutes for the printer to heat up and then 28 minutes to print the full design. Most of my printing experience was just watching a box being completely filled in with filament. It was really interesting to see the infill pattern once I got past the original wall thickness. I know I have used the same infill pattern for each project, but I still think it looks really cool. Here is a video of my design 3D printing:

[video](printing_video.MP4)

The total time spent printing was 48 minutes according to the end screen on the printer. Here is what the final design looked like:

<p align="center">
  <img src="final_print.jpg" alt="final_print" style="width:50%; height=auto"/>
</p>

My 3D printing process was my longest process. I found that dimensioning the holes using calipers is really optimistic, so I spent a lot of time playing around with the thickness and height of the supports. I did end up getting it to fit, and I am pretty happy with it.

#### Snapping Fit

My circuit board fit really well into my design. The pin supports are perfectly lined up, and locks in place really well. It doesn't move much when I shake it, and I can hold it all the way upside down. I am really happy with how it turned out. Here is a picture of the final snap:

<p align="center">
  <img src="final_snap.jpg" alt="demo" style="width:50%; height=auto"/>
</p>

## Mistakes Through Design Process

I have made a lot of mistakes through my design process. With my initial design, I made my shell thickness really thin. I made it 0.02in instead of 0.1in. I did this so that I could keep my original measurements as close as I could, but it ended up making my part really thin and flexible. I didn't really want this to happen, which is why I switched to the 0.1in. My next major mistake was only taking my initial measurements once. This caused my supports not to lineup, and leading me to retake my measurements two times. After I redid my measurements, everything fell into place correctly. The next mistake I made was making the larger supports a little too thick. When I put the snap fits on the supports, the circuit board couldn't snap into place. That is why I had to make my diameter 100 thousandths smaller than what I previously measured. The next mistake I made was printing the same design multiple times. I didn't change the name of my designs as I progressed, and I just exported the same file onto the same drive. I didn't realize it, but this printed the first design of that file name every time. So, I would print a failed design even though I changed my design three different times. The last major mistake was the orientation. With my orientation being horizontal, it makes it incredibly easy to snap the supports off the design. If I changed the orientation, it would make it a little more sturdy.

## Lessons Learned

With lots of failures comes a lot of lessons learned. The first thing that I learned from this project was how to refill the filament on a 3D printer. I have never had to refill the filament before, but I am glad I learned how to. I just have to purge the remaining material while feeding the new filament into the nozzle. I wait until the filament is the same color as the filament I am replacing it with. The next thing I learned is that I should measure things way more than once. It saves so much time and energy when everything is measured correctly on the first go around. I am not sure how common that is, as it is a common mistake, but it is crucial. The next lesson I learned was that I should be naming all of my prototypes different names. Either that or delete the file off the USB that I previously used. Doing so will actually print the product that I want. There was a point during this process where I printed the same design twice, and when I printed the design I made changes to, my support pins were not aligned anymore. It was very frustrating dealing with, but it is completely my fault that happened. The last thing I learned from this assignment is the importance of orientation. I keep my orientation defaulted, but it caused my pins to be super fragile. If I put just a little shear force on those pins, they would snap off. I would actually snap the pins from my failed designs while I was waiting for my next 3D print to finish.


