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

Now that I had all of my known values, I started solving for the important mechanical properties of my snap fit: length and bending stress. To get the length of my snap fit, I used the beam equation for the cantilever beam from A03 from the lecture portion of this class. P represents the transverse load, L represents the length, E represents young's modulus, I represents moment of inertia, and <img width="624" height="310" alt="image" src="https://github.com/user-attachments/assets/172c83a6-d263-46ff-bc6e-7914e354a6c0" /> is the max deflection I want.


### Design 2

