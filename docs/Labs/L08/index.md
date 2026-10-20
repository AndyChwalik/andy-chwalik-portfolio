# L8 - Design Something Useful

# Reading

Designers must ask smart questions throughout the design process to help clarify what the issue is and possible ways of fixing it. There are two different types of questions a designer can ask: Open-ended questions and closed questions. Open-ended questions are questions that help designers explore and clarify what is going on where closed questions are typical yes or no questions. A good question doesn't depend on the type of question where it focuses more on empowering creativity, challenging assumptions, encourage reflection, and often lead to breakthroughs. Good questions will find the root of the problem, challenge assumptions, and give a better understanding of context. There are many methods to asking questions, but one big is the 5 whys. This method has the designer ask why to a general statement 5 times. When you ask why 5 times, the theory is that you should have found the root issue after those5 questions.

# Problem Statement

The first idea that I had was some type of display area. I was thinking of creating a platform with a cutout of a circle. I will then place a separate circular piece in that cutout so that it will spin - displaying whatever you want to put on the platform. I didn't really like this idea though, so I started to think about stuff that is happening to me currently. I have become incredibly sick over the weekend, and I wish I had somewhere to put all of my miscellaneous stuff and medicine. I didn't really have anywhere to put it, so I think this will be a useful product I can use and other people going through a similar situation can use.

When I started to think of solutions for this problem, I thought of the same spinning platform. I can put a rod in the middle of the rotating disc, and spin the platform using this rod. This will allow me to store whatever I want on a circular platform while being able to easily access different items in storage. I also thought it may be a good idea to put some type of stopper for the rotating disc, so it can act as just a regular platform. 

# Design

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
      <img src="disc_rod_setch" alt="base" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        After I extruded the main part of the disc, I decided to create the rod in the middle. To make my dimensions consistent, and hopefully minimize printing errors, I decided to make the diameter of the road to be 0.25in.
      </div>
    </td>
  </tr>
  <tr>
    <td style="width:60%; text-align: center; vertical-align:middle;">
      <img src="disc_sketch.png" alt="base" style="width:100%; height:auto;">
    </td>
    <td style="width:40%; padding:28px; vertical-align:middle;"">
      <div style="font-size:14px;">
        To find the extrusion height I wanted to use, I had to make sure that it was taller than most of the products I would be putting on it. I measured the height of my ibuprofen bottle to be 2 and a fourth inches
      </div>
    </td>
  </tr>

