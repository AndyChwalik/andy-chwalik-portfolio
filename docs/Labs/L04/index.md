# L4 - Benchmark a parameter

## Parameter

The goal of Lab 4 is to show how some 3D printers can outperform or underperform different 3D printing design rules. An example of this is the overhang design rule. The general rule is to not print any 3D artifact over 45 degrees from the vertical axis. To test an individual 3D printing machine, it can print an artifact that has 1 less degree (44) or 1 more degree (46) to see how it performs. If the print isn't smooth at 44 degrees, that means the 3D printer underperforms for that specific test, and the designer should keep that in mind while designing different parts. The same thing can be said if the 3D printer outperforms the general rule. 

That was just an example though. Below is a graph of all of the different 3D printing design rules. The graph gives a little information about each design rule and then the parameters for each rule. Since I am going to be using the Prusa Core One 3D printer, I am looking at the "Fused deposition modeling" requirements. '

<p align="center">
    <img src="3D_Printing_Design_Rules.png" alt="View PDF" height="75%" width="auto">
</p>


I decided to test the horizontal bridges parameter. I chose the horizontal bridges parameter because I have tried to avoid any type of gaps or overhangs in my current designs. That is why they are all flat to the ground with small bumps or rounds on top of them. If I can test the limit of the Prusa Core One for horizontal bridges, I think it would give me more freedom when designing without supports for 3D models. 

## 3D Modeling

I am going to show 2 different designs. The first design was my first plan when going about this project. It unfortunately didn't turn out the way I wanted it to due to all of the bridges being the same height, making it hard to view the error, and there not being a big enough deviation from the 10mm rule. My second design is my revised plan, which fixes the issues of the first design. I will provide CAD files and STL files for both of the designs if you want to look into what I am talking about a little deeper.

## Design 1

Looking at the "3D Printing Design Rules", the rule for FDM is 10mm. For my testing, I will change the measurement by +/- 1mm. I will continue to do this until I have five different horizontal bridges on my 3D printing file. My final design will show horizontal bridges in measurements of 8mm, 9mm, 10mm, 11mm, and 12mm. Each horizontal bridge will have a 4mm gap between itself and the next horizontal bridge. With the wide range of measurements, it should give me a good idea of the capabilities of the Prusa Core One for this 3D design rule.

To eliminate risk of other failures unrelated to the design rule I picked, I decided to make the supports for the bridge a 5mm x 5mm square. I think this will provide enough support to keep the failure isolated towards the bridge design. The thickness of the actual bridge gap will be 2mm.

<table style="width:100%;">
  <tr>
    <td style="width:60%;">
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
    <td style="width:60%;">
      <img src="base_sketch_incorrect.png" alt="incorrect_base_sketch" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; text-align:center; vertical-align:middle;"">
      <div style="font-size:16px;">
        Once the base of my design was established, I could move onto the legs of the bridge gaps. To design the legs, I created a 5mm x 5mm box on the top left and top right corner of my base. Those represented my two extreme values. I then created another 5mm x 5mm box 8mm away from the top left and 12mm from the top right.
      </div>
    </td>
  </tr>
</table>
