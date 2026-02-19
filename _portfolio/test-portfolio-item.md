---
title: "First PLAntweight Combat Robot"
excerpt: "The path to NHRL begins with a single step."
header:
  image: /assets/images/Finished_Robot.jpg
  teaser: /assets/images/Finished_Robot.jpg
sidebar:
  - title: "El Comandante"
    #image: http://placehold.it/350x250
    #image_alt: "logo"
    text: "PLAntweight Robot"
  #- title: "Second Heading"
  #  text: "Longer Description"
gallery:
  - url: /assets/images/Filter_hack.jpg
    image_path: assets/images/Filter_hack.jpg
    alt: "placeholder image 1"
  - url: /assets/images/Filter_inside.jpg
    image_path: assets/images/Filter_inside.jpg
    alt: "placeholder image 2"
  - url: /assets/images/Finished_Filter.jpg
    image_path: assets/images/Finished_Filter.jpg
    alt: "placeholder image 3"
---

Let me walk you my journey of building a small, 1-pound (or 454-gram) robot, often called an "Antweight" or "Plastic Antweight." This is the perfect place to start, as it lets you learn all the core skills without a massive investment in parts.

Phase 1: Planning, Printing, and Sourcing Parts
Before even picking up a soldering iron, I first needed to choose a design. It's highly recommended to use a proven, open-source design, so I went with the "Force Knight" provided by [Team Malice](http://url-you-want-linked). Their designs are meant to work with the [SCAR PLANT Drive Kit](https://turnabot.com/products/scar-plant-turnakit) offered by Turnabot, simplifying the parts-sourcing task, and ensuring compliance with the SCAR tournament rules.

The SCAR PLAntweight class rules restrict us to PLA and PLA+, and we will be using both. The spinner weapon is printed solid out of PLA+. I experimented with using 99% concentric infill vs. using 100 perimeters/walls. Both printed fine but 99% concentric was more dimensionally accurate. We'll see which one is stronger! For the armor, I'm trying out different colors/formulations of PLA. The red is PLA-HS, which is stiffer and lighter, but may shatter more easily. It will be interesting to see which is better suited for the job!

<!--{% include gallery caption="This is a sample gallery to go along with this case study." %} -->
Phase 2: Soldering and Wiring
This is where we bring the electronics to life. First we build the Main Power Harness
This is the central trunk of your robot's electrical system.

  Prepare the Battery Lead: Solder your female XT30 connector to a length of red and black wire (about 4-6 inches). Crucially, slide a piece of heatshrink tubing onto each wire before soldering the connector! Once the joint is cool, slide the tubing over the exposed metal and shrink it with a heat gun (or careful use of a lighter) to prevent short circuits .

  Wire the Power Switch: Solder the red wire from your XT30 lead to one tab of the power switch. Solder the red wire that will go to your electronics (see step 3) to the other tab. The switch will now interrupt the positive power flow, acting as a master on/off .

  Step 3: Solder Motors to Malenki Board
  Solder the two wires from one motor to the output pads on one of your tinyESCs. The polarity (which wire goes where) will determine which way the motor spins. You can swap them later if needed .

Repeat for the second motor and ESC.


...Text about the finished project...

...include the video...