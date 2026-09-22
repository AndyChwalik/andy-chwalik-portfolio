# L5 - Design a Snap Fit

## Objective

The goal for Lab 5 was to create two separate parts that are able to connect with each other through a snap fit. What this means is you can slide the part into the other, have it lock in place, and then detach the parts by putting pressure on the connection point. An example would be any type of buckle on backpacks or a battery cover on remotes.

Snap fits use the property of elastic deformation in order to connect and disconnect. The pressure bends part of the connection, so you are able to slide the parts together. To lock them in place, there is a lip to stop the parts from coming out. To unlock them, you use the same elastic deformation properties to bend the locking material away, so that they can detach from each other.

<p align="center">
  <img src="example.jpg" alt="example_snap_fit" style="width:50%; height=auto"/>
  <br>
  <em>Here are some different types of snap fits and a visual representation if it is hard to picture through words.</em>
</p>

## Analyze

Before I think of possible snap fits, I want to make sure I have all of the variables for my design. I looked up the mechanical properties for PLA on Google, and I found a pdf from [Ultimaker](https://um-support-files.ultimaker.com/materials/2.85mm/tds/PLA/Ultimaker-PLA-TDS-v5.00.pdf). The young's modulus displayed found that PLA was around 3.25 GPa with a variance of 101 MPa. The listed yield strength is around 52.50 MPa with a variance of 0.9 MPa. Comparing this to other sites, it looks like the young's modulus ranges from 2.5GPa-3.5GPa and the yield strength ranges from 40MPa to 60MPa. For my project, I decided to use the middle of both of both of those: 3.0GPa, or 435000 psi, for young's modulus and 50GPa, or 7250psi, for yield strength. There had to be a transverse load of 0.25lbf - 5lbf, and there had to be an axial load of 5lbf - 10 lbf. The transverse load is the load required to unlock the objects from each other, and the axial load is the laod required to push the parts together. Everything had to be designed with a safety factor of 3.5.

Similar to my last project, I made two different designs. This wasn't on purpose, but I noticed at the end that my project was probably way too big and unnecessary for the assignment. I used the same math and process of development for both, but I will show the entire process for both designs. The second design is my final design, where there are some modifications at the end due to careless mistakes.

### Design 1

My first thought for a snap clip was a simple cantilever snap fit, similar to a buckle. I didn't want to make a buckle exactly, so I tried to think of different designs I wanted to do. My first thought was to make a box to hold all of the 3D prints we will be making throughout the semester. It will have a the snap fit as the latch for the box, so I can open and close it similar to how you open and close a chest.

This box was supposed to hold all of my 3D prints, so I was thinking I had to make it pretty big in dimensions. I already knew the young's modulus, yield strength, safety factor, and material I would be using; but, I had to choose my transverse load, axial load, base, width, and maximum deflection. Similar to my decisions for young's modulus and yield strength, I chose the middle points for the transverse load (2.5lbf) and axial load (7.5lbf). The maximum deflection was a little bit more difficult for me to decide.

For me to decide on my maximum deflection, I had to gauge how big I wanted my latch to be. In other words, I needed to decide on my base and width of my snap fit. I was working with inches, and I tried to use easy to manufacture measurements. I made the width of my clip 0.25in and the base of my clip 0.50in to try and adhere to the easy to manufacture measurements. The next measurement down was 1/8in, so that's what I decided to make my maximum deflection.

#### Paper Calculations

##### Length

Now that I had all of my known values, I started solving for the important mechanical properties of my snap fit: length and bending stress. To get the length of my snap fit, I used the beam equation for the cantilever beam from A03 from the lecture portion of this class. P represents the transverse load, L represents the length, E represents young's modulus, I represents moment of inertia, and δ is the max deflection I want. When I solve for L, and plug in the known values, I get the length of my snap fit to be 3.49in. This is longer than I expected, but I was trusting the process.

##### Free-Body-Diagram
Once I had the length of my snap fit, I decided to create free-body-diagrams of the clip and what the clip is connected to. The clip has the transverse load acting on it, creating a moment about the clip. There is also the axial force acting on the clip from the connection point. The axial load doesn't affect the moment as it is apart of the axis I was taking the moment from. 

The connection point for the clip was a simple free-body-diagram since the axial force is the only thing that really affected it. The transverse load affected it slightly, but I didn't think it would be severe enough to take any major considerations into.

I also drew some isometric pictures to get a general idea of what I was expecting when 3D printing this material. The box would be 6in by 12in, meaning that it is too large for the 3D printer to print, but I didn't know that at the time. It would also take up a lot of material.


##### Bending and Axial Stress

Now that I had my FBD's down, I could start to calculate the bending stress and the axial stress of my snap fit. To calculate bending stress, I used the same equation I used in A04 for the lecture portion of this class. Since I know more of the variables, I don't have to break it down quite as far as A04, but I am still using it to calculate bending stress.

To make sure that this bending stress won't exceed my safety factor, I had to calculate the allowable stress for my snap fit. To do this I used the simple equation of yield strength/safety factor.

Comparing my calculated bending stress to my allowable stress, my design should be well in the specifications. 

I did the same thing with axial stress, but used the axial load instead of the transverse load from the bending stress calculations. This gave me a super low axial stress. When compared to the allowed stress, I am well under the specifications once again.

#### CAD Modeling

<table style="width:100%;">
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_equations.png" alt="equations" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        The first thing I did was fill out the global variables and equations that I will be using to design my snap fit. I put in every single known variable that would be useful while designing.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_base_box.png" alt="base_dimensions" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        The first thing I did after the equations was make an outline of the box that would be holding all of my 3D designed parts. Based on my drawings, this would be 6in x 12 inq
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_base_extrusion.png" alt="base_extrusion" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I wasn't sure how tall I should make it, but I ended up making it the same as the width of the box for consistency. I also thought it would've been good for stacking 3D prints on top of each other.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_base.png" alt="base_shell" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        After extruding the basic shape, I used the shell tool to make the box empty. It will allow me to use it for storage and it will save on material. I decided to make the shell 1/8in.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_connection_base.png" alt="hole_length" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        Once I had my hollowed out box, I moved onto the connection point. I knew the length of the snap fit would be 3.49in, so I made sure to make the hole 3.49in from the top of the box. I did this through the global variable I made.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_connection_centered.png" alt="hole_connection" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        Once I had the length down, I then used the global variables for width and base to create the dimensions for the hole. I also made sure that the hole was centered in the middle of the box, so that it would be easy to line up the snap fit.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_connection_extrusion.png" alt="connection_extrusion" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        After the hole was dimensioned correctly and centered, I extruded it through the whole object. Doing so finished the design for the main base of the snap fit.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_base_top_extrusion" alt="design1_top" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        To design the top of the snap fit, I copied the equations and global variables from the first design to this new part file. I then copied the base dimensions of base to the top of the box. I decided to extrude it only 2in to give it a more chest feel to it.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_base_top_shell.png" alt="top_shell" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I used the shell tool again to hollow out the top. I made sure that the thickness of the walls were the same as the base of the snap fit.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_extrusion.png" alt="clip_base_extrusion" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        After finishing the hollowed out top, I moved onto actually designing the clips that will connect the two boxes together. To do this, I created a box with the dimensions of the width and base of the clip at the very edge of the hollowed out top.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_clip_extrusion.png" alt="clip_extrusion" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        Once this part was extruded, I had the correct dimensions for the clip, and I could extrude this extension to the length I calculated earlier. I used the length global variable for this.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_clip_catch_extrusion.png" alt="catch_extrusion" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I then started to create a catching mechanism so that the clip snap into place. To do this, I made another box, the dimensions being the base and width, at the very edge of the clip. I then extruded this by 0.15in. I chose 0.15in so that it would be easier to detach once it was snapped together.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_clip_catch_angle.png" alt="clip_catch_angle" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        To add some angle to the design, I added a 44 degree angle at the catch point. I am actually not sure what it does, but I see it pretty often on these type of snap fits. 
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_clip_catch_angle_extrusion.png" alt="clip_catch_angle_extrusion" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I extruded this angle through the entire catching mechanism.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_mirror.png" alt="mirror" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        My snap clip is now finished. Instead of repeating all of the steps I just did on the other side, I created a plane in the middle of my object so that I could mirror it to the other side with the exact same dimensions. This also makes it so that both clips dimensions will change together if I decide to change them. It also rounds out the design for the top of my part.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="design1_assembly.png" alt="assembly" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        I put both of them in an assembly to get a good idea of what everything will look like together. I made the top of the clip catch coincident with the top of the hole on the base and I made the walls of those two objects coincident to each other. This gave me a picture of what my model would look like all put together.
      </div>
    </td>
  </tr>


### Design 2

