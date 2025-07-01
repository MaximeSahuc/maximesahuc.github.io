+++
title = "Making invisible IC sockets"
summary = "Method for making custom and invisible IC sockets for PCB."
tags = ["diy", "electronic", "pcb"]
date = 2025-06-30
draft = false
toc = true
+++

## Context

For context, I'm currently building an electronic clock that would need some ICs.
Wishing the clock to be repairable, I opted to use some IC sockets to be able to replace some components.

Wanting also to keep a good aesthetic for this project, I don't want big and ugly sockets on my board.
After racking my head for a simple and cost effective solution, I remembered the female header pins I had purchased a while ago but never used because they were too small for standard 2.54mm male pins to fit in.
But, it turns out that these pins are the perfect hole size for components like ICs and a lot of passives!

## Making the socket

The main advantages of this solution are the `aesthetic` but also the ability to make `sockets for anything` _(as long as the component legs fit in the socket holes)_!
In this post I will show how to make an _invisible_ socket for an 8 pin IC.

{{<details summary="See the list of items I used">}}
- Smalls DIP female pins, similar to [these ones](https://www.digikey.com/en/products/detail/aries-electronics/08-0518-10/4206287)
- 1.8mm drill bit
- Small drill and pliers
- Heat-resistant tape
- Soldering iron and tin
{{</details>}}

<br>

Here is a picture of the small DIP header female pins I used:

![Image of the female header pins](./images/dip_female_header_pins.jpg)

### Extracting the header pins

The first step is to remove the female headers from their plastic enclosure using pliers.

![Image of the exrtacted female header pings](./images/female_headers_extracted.jpg)

### Drilling the PCB

Now we can make room for these header pins by drilling 1.8mm holes in the PCB.

![Image of the 1.8mm drill bit](./images/drill_bit.jpg)

Here is what the drilling looks like for an 8 pin IC:

![Image of the drilled holes](./images/pcb_holes_drilled.jpg)

### Inserting the header pins

Once the socket holes are drilled, you can press fit the female header pins into their respective holes.
It may be necessary to use some heat-resistant tape to prevent the pins from falling.

Here is a picture of the inserted header pins:

![Image of the inserted header pins from the top](./images/pcb_female_pins_inserted_top.jpg)

And here is the bottom view:

![Image of the inserted header pins from the bottom](./images/pcb_female_pins_inserted_bottom.jpg)

Note that if you have vertical space constraints, you can cut the end of the pin before soldering it.
But be careful to cut __only the end__ of the pin and not the hole where the IC pin will insert!

### Soldering the pins

Now it's time to solder the pins to the PCB!
As the drilling removed the copper layer around the holes, it's necessary to make a solder bridge between the header pin and an adjacent pad.

![Image of the soldered header pins from the bottom](./images/pcb_pins_soldered_bottom.jpg)

And here's what it looks like from the top:

![Image of the soldered header pins from the top](./images/pcb_pins_soldered_top.jpg)

## Final result !!

As you can _(or cannot)_ see, the socket is pretty much invisible from the top!

![Image 1 of the final PCB](./images/final_result_1.jpg)

![Image 2 of the final PCB](./images/final_result_2.jpg)

![Image 3 of the final PCB](./images/final_result_3.jpg)

And the best part about this solution is that I can now replace components without worrying about desoldering them an hour after soldering, because I burned them  ಠ_ಠ...

---
