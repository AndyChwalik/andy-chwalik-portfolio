# L4 - Benchmark a parameter

## Parameter

The goal of Lab 4 is to show how some 3D printers can outperform or underperform different 3D printing design rules. An example of this is could be the overhang design rule. The general rule is to not print any 3D artifact over 45 degrees from the vertical axis. To test an individual 3D printing machine, it can print an artifact that has 1 less (44) or 1 more degree (46) to see how it performs. If the print isn't smooth at 44 degrees, that means the 3D printer underperforms for that specific test, and the designer should keep that in mind while designing different parts. The same thing can be said if the 3D printer outperforms the general rule. 

That was just an example though. Below is a graph of all of the different 3D printing design rules. The graph gives a little information about each design rule and then the parameters for each rule. Since I am going to be using the Prusa Core One 3D printer, I am looking at the "Fused deposition modeling" requirements. 

![3D_Printing_Design_Rules](3D_Printing_Design_Rules.pdf)

### Analyze

I decided to test the horizontal bridges parameter. I chose the horizontal bridges parameter because I have tried to avoid any type of gaps or overhangs in my current designs. That is why they are all flat to the ground with small bumps or rounds on top of them. If I can test the limit of the Prusa Core One for horizontal bridges, I think it would give me more freedom when designing without supports for 3D models. 

Looking at the "3D Printing Design Rules", the rule for FDM is 10mm. For my testing, I will change the measurement by +/- 1mm. I will continue to do this until I have five different horizontal bridges on my 3D printing file. My final design will show horizontal bridges in measurements of 8mm, 9mm, 10mm, 11mm, and 12mm. Each horizontal bridge will have a 6mm gap between itself and the next horizontal bridge. With the wide range of measurements, it should give me a good idea of the capabilities of the Prusa Core One for this 3D design rule.
