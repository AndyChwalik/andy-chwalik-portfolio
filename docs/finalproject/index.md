# Final Project – [Topic]

## Objective

Choose a problem that can be addressed with 3D printing/laser cutting and develop an initial design concept.

## Part 1

### Research

#### Spiral Design Process

While researching the spiral design process, I found a lot of different websites that promoted the spiral model for software engineers. When I looked up mechanical engineering, I was left with mechatronics a result. This doesn't mean that it is only used by tech people, but I thought it was interesting that it was promoting this model for software engineers rather than for general use.

<p align="center">
  <img src="spiral_model.png" alt="spiral model" style="width:100%; height=auto"/>
</p>

The spiral design process is a design process that likes to think of different design ideas while mitigating risks at the same time. It is a very powerful design model because each design that you come up with should build on the last, making a better product in the end. There are four main phases to the spiral design process: planning, risk analysis, development, and evaluation.

The planning phase is the first phase you will go through, and this primarily explores the requirements, constraints, and possible ideas for the problem you're trying to solve. This makes me think of what we are doing for part 1 of this project, since we aren't trying to have a solution to our problem yet. 

Risk analysis is the second phase, and this is where you'll start on the actual design. You can go through this with you're own design process, but general strategies include creating design matricies and building/testing multiple prototypes. You will use the prototypes and data collected form this phase to then move onto the next phase.

Development is the third phase, and this is where you will create the final product of your project. I saw from a few different sources that this is where you have a proof of concept to validate your design before committing to the final product. The proof of concept seems like a final check to the whole design.

The last phase is evaluation. The evaluation step is where you look at your final product and compare it to the criteria you set in the planning phase. Does the design meet the requirements you set? Does the design work as intended? Are there any failures/flaws that are noticeable and can be improved upon? These are the types of questions you'll ask yourself during this phase.

This design process is useful for this project because it will allow me to identify weaknesses in my designs early, leading to constant improvement and a better final product. Even if I don't fully use this design process, I would like to at least incorporate the design matrix into my design process. I think this will be helpful in removing bias in designs while giving what should be the best design.

#### FDM Anisotropic

FDM anistropic parts refer to how some areas of the part are mechanically weaker compared to others due to the way it was 3D printed. When I research it, the main reason for this happening is the layer by layer process along the z-axis. MLC lists three properties that make this the main reason: molecular structure, mechanical properties, and infill patterns.

Plastic polymers are formed from chemical chains, which grow stronger when melted. This is good when 3D printing since filament has to be melted in order to be 3D printed; however, the heat from the layers proceeding may only heat up portions of the layer before it, creating weak points in the material.

The mechanical property that can produce anisotropic parts is the layer by layer process 3D printers go through. The layer by layer process will create these visible lines between each layer. Those visible lines are potential stress points in the design and could cause the part to fail. Cracks can form on these lines, separating that layer from the rest of the design.

The infill pattern selected will dictate how strong your part will actually be. Since FDM parts aren't completely solid, the infill pattern and percentage will be the only support your part will have in the middle. If the wrong infill pattern is selected, it could cause higher stresses than normal, causing the part to break.

To avoid these weaknesses, you can adjust the printer settings for temperature and speed to enhance the molecular bonds, align the design in a certain way to minimize the visible lines left by the 3D printer, and research what the best infill will be for the job you want that part to do.

#### SLA Shrinkage

SLA shrinkage is where your part shrinks or deforms during the curing process of SLA printing. The material you're using affects how much your part will shrink. According to BFoxDoc, ABS will shrink about 8% and PLA will shrink only 2%. The two main reasons for the shrinkage is due to thermal expansion/contraction and changes at the molecule level.

SLA uses a laser to run over liquid resin, causing the resin to solidify in whatever pattern the laser went over it in. This process is an exothermic reaction, meaning that a lot of heat is generated. The change from hot to cold can cause the part to warp and deform if not designed properly. This process happens again once you try to bake your part during the curing process. This means there are two parts in the SLA design process that can shrink your part through thermal expansion and contraction.

Looking at it at the molecular level, the resin changes from small molecules to long-chain polymers. During this process, shrinkage is impossible to avoid.

Based on my previous designs for SLA and my research, I really need to add a certain percentage onto my dimensions in order for my part to be the correct size. I haven't had a successful print using SLA yet, so I really need to pay attention to the material properties. If I use SLA, I will need to look up the shrinkage rate for grey v5 or clear v5. It depends which I decide to use. I also think it is good to leave me part by itself after curing to let the sticky surface kind of dissipate before testing.

#### Laser Cut Kerf

Laser cut kerf is the material the laser burns away while it cuts through whatever material you're using. The kerf can change a lot depending on the machine you are using and the material you are using.

The machine being used is important to take into consideration since the quality of laser can vary greatly from machine to machine. The higher quality lasers will have a smaller kerf than the less quality lasers, and is important to take into considerations.

The material is what really affects the kerf, since this changes the kerf on the same machine multiple times. Not only do the mechanical properties of that material come into play, but also the thickness of that material. The thicker that material is, the harder it will be for the laser to cut through it. This could cause more material to be burned away than normal, increasing the kerf. Here is a table of general kerf sizes from CutLaserCut
<p align="center">
  <img src="kerf_tendicies.png" alt="kerf table" style="width:100%; height=auto"/>
</p>

If you don't take the kerf into account, your parts may not fit the way you want them to fit if they fit together at all. We didn't really have issues with our laser cuttting project, however this made our smaller parts not fit as well as we wanted them to. 

#### Resources

- [https://teachingagile.com/sdlc/models/spiral](https://teachingagile.com/sdlc/models/spiral)
- [https://www.projectmanager.com/blog/proof-of-concept-definition](https://www.projectmanager.com/blog/proof-of-concept-definition)
- [https://blog.unisquareconcepts.com/designing/spiral-design-thinking-process-and-its-phases/](https://blog.unisquareconcepts.com/designing/spiral-design-thinking-process-and-its-phases/)
- [https://www.mlc-cad.com/resources/3d-printing/why-fdm-3d-prints-are-weaker-on-the-z-axis-anisotropy-explained/](https://www.mlc-cad.com/resources/3d-printing/why-fdm-3d-prints-are-weaker-on-the-z-axis-anisotropy-explained/)
- [https://facfox.com/docs/kb/one-common-failure-for-sla-the-material-deformation](https://facfox.com/docs/kb/one-common-failure-for-sla-the-material-deformation)
- [https://formlabs.com/support/Warping-SLA/](https://formlabs.com/support/Warping-SLA/)
- [https://www.machinemfg.com/things-you-should-know-about-laser-cut-kerf/](https://www.machinemfg.com/things-you-should-know-about-laser-cut-kerf/)
- [https://cutlasercut.com/drawing-resources/expert-tips/laser-kerf/](https://cutlasercut.com/drawing-resources/expert-tips/laser-kerf/)




## Part 2
