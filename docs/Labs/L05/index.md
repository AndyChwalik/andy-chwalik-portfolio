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

Before I think of possible snap fits, I want to make sure I have all of the variables for my design. I looked up the mechanical properties for PLA on Google, and I found a pdf from [Ultimaker](https://um-support-files.ultimaker.com/materials/2.85mm/tds/PLA/Ultimaker-PLA-TDS-v5.00.pdf). The young's modulus displayed found that PLA was around 3.25 GPa with a variance of 101 MPa. The listed yield strength is around 52.50 MPa with a variance of 0.9 MPa. There had to be a transverse load of 0.25lbf - 5lbf, and there had to be an axial load of 5lbf - 10 lbf. The transverse load is the load required to unlock the objects from each other, and the axial load is the laod required to push the parts together. Everything had to be designed with a safety factor of 3.5.

