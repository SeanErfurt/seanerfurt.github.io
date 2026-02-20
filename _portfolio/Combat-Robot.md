---
title: "My First PLAntweight Combat Robot"
excerpt: "The path to NHRL championships begins with a single step."
header:
  image: /assets/images/Robot_thumb.jpg
  teaser: /assets/images/Robot_thumb.jpg
sidebar:
  - title: "El Comandante"
    #image: http://placehold.it/350x250
    #image_alt: "logo"
    text: "PLAntweight Robot"
  #- title: "Second Heading"
  #  text: "Longer Description"
gallery:
  - url: /assets/images/print1.jpg
    image_path: assets/images/print1.png
    alt: "Spinner & Mount"
  - url: /assets/images/print2.jpg
    image_path: assets/images/print2.png
    alt: "Armor"
  - url: /assets/images/print3.jpg
    image_path: assets/images/print3.png
    alt: "Spinner2"
---

Let me walk you through my journey of building a small, 1-pound (or 454-gram) robot, often called a "PLAntweight" or "Plastic Antweight" bot. This is the perfect place to start, as it lets me learn all the core skills without a massive investment in parts.

<h2>Phase 1: Planning and Sourcing Parts</h2>

![image-FK](/assets/images/Force_Knight.png)

Before even picking up a soldering iron, I first needed to choose a design. It's highly recommended to use a proven, open-source design for your first build, so I went with the "Force Knight" provided by [Team Malice](https://teammalice.com/index.php/scar-kit-and-spares/scar-plastic-antweight-electronics-kit/). Their designs are meant to work with the [SCAR PLANT Drive Kit](https://turnabot.com/products/scar-plant-turnakit) offered by Turnabot, and they offer a standard SCAR spinner weapon kit too, simplifying the parts-sourcing task, and ensuring compliance with the SCAR tournament rules.

<h2>Phase 2: Printing the Rest</h2>

{% include gallery %}

The SCAR PLAntweight class rules restrict us to PLA and PLA+, and we will be using both. The spinner weapon is printed solid out of PLA+. I experimented with using 99% concentric infill vs. using 100 perimeters/walls. Both printed fine but 99% concentric was more dimensionally accurate. We'll see which one is stronger! For the armor, I'm trying out different colors/formulations of PLA. The red is PLA-HS, which is stiffer and lighter, but may shatter more easily. It will be interesting to see which filament is better suited for the job!

<h2>Phase 3: Soldering and Wiring</h2>

![image-wires](/assets/images/Malenki_wiring_diagram.png)

This is where we bring the electronics to life. It's important to lay everything out using your chassis so that you can cut your wires to length (with a little extra to spare). I also tried several methods to make the connections modular, durable, and easy to repair too.

1. Prepare the Battery Lead: 

Solder your female JST connector's black wire to the board where it's labelled "- PWR" on the Malenki board. Remember to slide a piece of heatshrink tubing onto each wire before soldering the connector! Once the joint is cool, slide the tubing over the exposed metal and shrink it with a heat gun to prevent short circuits.

2. Wire the Power Switch: 

Solder the red wire from your JST lead to one tab of the power switch. Solder a red wire that will go to the Malenki's "+" pad to the center tab. The switch will now interrupt the positive power flow, conforming to safety rules.

3. Solder Motors to Malenki Board: 

Solder two wires from one N20 motor to another. Then solder another 2 wires to the corresponding output pads (L, R) on the board. Repeat for the other side. Once assembled, we can test the motors and switch polarities if they are spinning in the wrong direction. I used [Team Run Amok's Combat Robot Mixer Fixer](http://runamok.tech/RunAmok/mixfix4.html) program to help diagnose my mixing issues. We also solder some 2mm banana connectors to connect our brushless weapon motor to the brushless ESC. Lastly we connect the red and black ESC wires to the Malenki "W" pads (I used eyelets with nyloc nuts here), and run the white ESC signal wire to the lower PWM pad.

<h2>Phase 4: Assembly and Testing</h2>

![image-inside](/assets/images/Robot_inside.jpg)

Team Malice already did a great job documenting the assembly process for Force Knight, so I will just [link that here](https://instructions.online/?id=10785-force%20knight%20-%20updated). Once the polarity of the drive motors is fixed, and we've tuned our transmitter mixing, we are ready for a test drive! Stay tuned for that video soon.

![image-finish](/assets/images/Finished_Robot.jpg)

<!-- include the video? -->