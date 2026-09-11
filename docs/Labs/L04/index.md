# L4 - Benchmark a parameter

## Parameter

The goal of Lab 4 is to show how some 3D printers can outperform or underperform different 3D printing design rules. An example of this is the overhang design rule. The general rule is to not print any 3D artifact over 45 degrees from the vertical axis. To test an individual 3D printing machine, it can print an artifact that has 1 less degree (44) or 1 more degree (46) to see how it performs. If the print isn't smooth at 44 degrees, that means the 3D printer underperforms for that specific test, and the designer should keep that in mind while designing different parts. The same thing can be said if the 3D printer outperforms the general rule. 

That was just an example though. Below is a graph of all of the different 3D printing design rules. The graph gives a little information about each design rule and then the parameters for each rule. Since I am going to be using the Prusa Core One 3D printer, I am looking at the "Fused deposition modeling" requirements. '

<p align="center">
    <img src="3D_Printing_Design_Rules.png" alt="View PDF" height="75%" width="auto">
</p>


I decided to test the horizontal bridges parameter. I chose the horizontal bridges parameter because I have tried to avoid any type of gaps or overhangs in my current designs. That is why they are all flat to the ground with small bumps or rounds on top of them. If I can test the limit of the Prusa Core One for horizontal bridges, I think it would give me more freedom when designing without supports for 3D models. 

## Designing

I am going to show 2 different designs. The first design was my first plan when going about this project. It unfortunately didn't turn out the way I wanted it to due to all of the bridges being the same height, making it hard to view the error, and there not being a big enough deviation from the 10mm rule. My second design is my revised plan, which fixes the issues of the first design. I will provide CAD files and STL files for both of the designs if you want to look into what I am talking about a little deeper.

## Design 1

### 3D Modeling

Looking at the "3D Printing Design Rules", the rule for FDM is 10mm. For my testing, I will change the measurement by +/- 1mm. I will continue to do this until I have five different horizontal bridges on my 3D printing file. My final design will show horizontal bridges in measurements of 8mm, 9mm, 10mm, 11mm, and 12mm. Each horizontal bridge will have a 4mm gap between itself and the next horizontal bridge. With the wide range of measurements, it should give me a good idea of the capabilities of the Prusa Core One for this 3D design rule.

To eliminate risk of other failures unrelated to the design rule I picked, I decided to make the supports for the bridge a 5mm x 5mm square. I think this will provide enough support to keep the failure isolated towards the bridge design. The thickness of the actual bridge gap will be 2mm.

<table style="width:100%;">
  <tr>
    <td style="width:60%; text-align: center">
      <img src="base_sketch_incorrect.png" alt="incorrect_base_sketch" style="width:100%; height:auto;">
        <img src="base_sketch_correct.png" alt="correct_base_sketch" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; text-align:center; vertical-align:middle;"">
      <div style="font-size:16px;">
        To start 3D modeling, I created a small base layer to put all of the bridge gaps on top of. I hope this will minimize printing errors, and properly show the results of the test. When I originally did this, I tried adding all of the length values in my head, and I got the incorrect dimensions. So, I had to adjust the length of my base layer from 39mm to 41mm. The bottom image shows the correct dimensions for what I am testing.
      </div>
    </td>
  </tr>
    tr>
    <td style="width:60%; text-align: center">
      <img src="beam_dimensions.png" alt="initial_beam_dimensions" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; text-align:center; vertical-align:middle;"">
      <div style="font-size:16px;">
        Once the base of my design was established, I could move onto the legs of the bridge gaps. To design the legs, I created a 5mm x 5mm box on the top left and top right corner of my base. Those represented my two extreme values. I then created another 5mm x 5mm box 8mm away from the top left and 12mm from the top right. Those dimensions are the bridge gap dimensions. 
      </div>
    </td>
  </tr>
    tr>
    <td style="width:60%; text-align: center">
      <img src="beam_dimensions_continued.png" alt="beam_dimensions_continued" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; text-align:center; vertical-align:middle;"">
      <div style="font-size:16px;">
        Now that I have the two leg ends of my design, I can work on offsetting those points to get the rest of the bridge gaps. Since all of my bridge gaps had the same starting position, I was able to create the 5mm x 5mm boxes along the top 4mm apart from each other. After doing so, the space on the top part of my base plate was all used up because the base plate was designed for 5mm x 5mm legs that were 4mm apart from each other. Since all of the starting positions for the bridge gaps were in place, I wanted to start on creating that bridge gap on the base plate. I was able to accomplish this in the same way I did the first bridge gap and the last bridge gap (creating another 5mm x 5mm box directly across from the starting point and making sure that the starting support leg and the final support leg had the proper bridge gap distance between them).  
      </div>
    </td>
  </tr>
    tr>
    <td style="width:60%; text-align: center">
      <img src="beam_dimensions_finished.png" alt="beam_dimensions_finished" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; text-align:center; vertical-align:middle;"">
      <div style="font-size:16px;">
        I continued this process for all of my bridge gaps. The end goal for this process is to have the support legs set in place so that I could extrude all of the support legs to the same height, and then actually create the bridge gaps across the leg supports. This is shown in the final sketch for the support legs.
      </div>
    </td>
  </tr>
    tr>
    <td style="width:60%; text-align: center">
      <img src="beam_extrusion.png" alt="support_legs_extruded" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; text-align:center; vertical-align:middle;"">
      <div style="font-size:16px;">
        I wasn't really sure what height I wanted to extrude it to, but I wanted the print to not take so long, so I decided to extrude all of the support legs by 5mm. I thought that it would be a big enough gap to tell if the 3D print failed while maintaining a low print time. 
      </div>
    </td>
  </tr>
    tr>
    <td style="width:60%; text-align: center">
      <img src="bridge_sketch1.png" alt="sketch_for_one_bridge_gap" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; text-align:center; vertical-align:middle;"">
      <div style="font-size:16px;">
        My next thought was to create a sketch on the support legs that will be the width and height I wanted my bridge gaps to be. Since they're attached to the support legs, the width will be 5mm, but I decided to go with 2mm for the height. I chose 2mm because I thought with a thinner design, it would show the failure of the different bridge gaps more clearly. I also had to do each of these sketches individually since they will all be extruded to different values, since the lengths of the bridge gaps will vary by 1mm. The picture shown shows the process for the first support leg.
      </div>
    </td>
  </tr>
    tr>
    <td style="width:60%; text-align: center">
      <img src="bridge_sketch_all.png" alt="sketch_for_all_bridge_gap" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; text-align:center; vertical-align:middle;"">
      <div style="font-size:16px;">
        Here are all of the sketches drawn on the different support legs. They all have the same dimensions, but as stated earlier, they will be extruded to different values due to the different bridge gap lengths.
      </div>
    </td>
  </tr>
    tr>
    <td style="width:60%; text-align: center">
      <img src="bridge_extrusion1.png" alt="extruding_beam_one" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; text-align:center; vertical-align:middle;"">
      <div style="font-size:16px;">
        With all of the bridge gap sketches in place, I started extruding them. The first bridge gap will be extruded by 8mm, since that was the length I have been designing this artifact for. The rest of the gaps will be extruded by exactly 1mm greater until I reach the 12mm I wanted to test. 
      </div>
    </td>
  </tr>
    tr>
    <td style="width:60%; text-align: center">
      <img src="finished_model.png" alt="finished_model" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; text-align:center; vertical-align:middle;"">
      <div style="font-size:16px;">
        Once all of the bridge gaps were extruded, I had my finished product. I was pretty happy with it, since that is what I was picturing when I first started designing the artifact.
      </div>
    </td>
  </tr>
</table>

### Preprocessing

I moved onto PrusaSlicer after saving my CAD model as an stl file. When I imported my model, it came in sideways again. I am not sure why this keeps happening because I thought I designed my part on the top plate, but it is a simple fix. All I had to do was just rotate the design by 90 degrees, and the design should be flat on the bed. 

<table style="width:100%;">
  <tr>
    <td style="width:50%; text-align: center">
      <img src="initial_orientation.png" alt="initial_orientation" style="width:100%; height:auto;">
    </td>
    <td style="width:50%; text-align: center"">
      <img src="fixed_orientation.png" alt="fixed_orientation" align="center"; style="width:100%; height:auto;">
    </td>
  </tr>
