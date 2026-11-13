# L9 – Laser Cutter

**Group:** Eshan Thaker and Andy Chwalik

## Objective

- Evaluate laser cutting as a viable manufacturing process. You will select and record machine settings, and explain the process's strengths and limits compared with FDM printing.

- Measure laser kerf and actual material thickness, and apply both as engineered allowances so your joints fit reliably across the whole sheet.

- Translate a parametric 3D model into 2D cut files, then back into a working 3D assembly.

## Analyze

### Step 1: Measure the Material  

For this part of the project we had to take a pair of calipers and measure the thickness of the wood board. We did this 3 times, and then measured the average of those thicknesses. This is important process because everything that is manufactured has some type of error that we need to account for. The board we were using is 3mm, so we should expect 0.118in. 

<div align="center">

| | Thickness 1 | Thickness 2 | Thickness 3 | Average |
|---|---|---|---|---|
| Measurement | 0.114in | 0.117in | 0.111in | 0.114in |

</div>

After measurements our average ended up being 0.114in. This is a little below what we expected, but there are a lot of errors that could've occurred. Like I said before, the manufactured pieces already have slight error, so that could be a reason for the slightly lower measurement. The other error I was thinking about is human error. We could've been squeezing the calipers too hard so we could've gotten lower values because of that. I am sure there are more reasons, but those are the main two I can think of.

### Step 2: Measure the Kerf

The next step is to measure the kerf. We didn't really know what the kerf was before this assignment, so it is important to talk about what the kerf is. While laser cutting, the laser will burn through a small amount of material to cutout whatever design you want. That small material the laser cutter cuts out is what we call the kerf. To measure the kerf, we will make a 15mm x 15mm, 0.591in x 0.591in, square and then measure the length and width with calipers. We will then measure the measured values from what's supposed to be the actual value to find what our kerf is.

To setup the square, I drew a sketch of a 15mm x 15mm box in SolidWorks. I then opened the solidworks file in Inkscape. This will show me what the cut will look like beforehand. Once everything looked good, I printed my inkscape file into Epilog. When in epilog I went to the material properties and selected vector for the process type. This will mean that I am cutting out my design rather than engraving. I also made sure to specify a 3mm wooden board and kept the default settings for that.

<table style="width:100%;">
  <tr>
    <td style="width:50%; align="center"">
      <div style="font-size:18px; text-align: center;">
        <b>Inkscape view for our square</b>
      </div>
      <img src="square_inkscape.png" alt="square inkscape" style="width:100%; height:auto;">
    </td>
    <td style="width:50%; align="center"">
      <div style="font-size:18px; text-align: center;">
        <b>Epilog view for our square</b>
      </div>
      <img src="square_epilog.png" alt="square epilog" style="width:100%; height:auto;">
    </td>
  </tr>
</table>

Here are our measured values from the calipers after laser cutting

<div align="center">

| | Width (x-axis) | Length (y-axis) | Average |
|---|---|---|---|
| Measurement | 0.584in | 0.582in | 0.583in |
| Kerf | 0.007in | 0.009in | 0.008in |

</div>

After cutting out our square and measuring it, we found a kerf of 0.007in in the width and 0.009in in the length. We averaged these two values together to get the kerf we will be using in the rest of this assignment: 0.008in.

### Step 3: Run a Fit Test

This project requires to fit different cutout pieces together, so we needed to find out what the best measurements would be for that. In order to do that, we made a coupon that will test different measurements to give us a clearance for our design based on the cutout square from the previous step.

The coupon will have five different measurements. The middle slot will be what our measured thickness is supposed to be: 0.114in. The slots to the right increase by 1 kerf all the way to the end. So the far right slot should add 2 kerf onto the average thcinkess: 0.13in. The reverse is true when going to the left. It will subtract by 1 kerf all the way to the end. So the far left slot will be subtracting2 kerf from the average thickness: 0.098in. 



## Decide


## Communicate

