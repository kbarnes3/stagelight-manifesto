---
layout: default
title: Getting Started - Stagelight Manifesto
---

Getting Started
===============
{{ site.name }} is broken down into phases. After each phase, it's possible to validate or show off what you've
done so far. Phase one is focused on getting your lights connected to your Raspberry Pi and cycling through test patterns.
Unfortunately, the first phase also requires the most purchasing and a fair amount of soldering. This phase will walk you
through picking out the right components, installing all the software, and hooking everything up, first on a breadboard
and then on a soldered circuit board.

# Purchase list
For purchases, this guide will try to provide direct links to items as well as what features are important if you want
to look for different items to better meet your needs. Due to the focused nature of this project, the required specs will
be pretty rigid. Some items are only used in breadboarding; they can be omitted if you prefer to skip these steps.

1. [Raspberry Pi 3](https://www.adafruit.com/products/3055)

    If you have a Raspberry Pi 2 sitting around, it should also work but it isn't yet tested completely. Due to the software
distribution used, only Raspberry Pi's are supported and tested. There are many bundles available online that contain
a Pi as well as many of the below items, as well as many items not needed for {{ site.name }}.
Some of these bundles might be cost effective for you.

1. Micro SD Card

    {{ stie.name }} doesn't have very demanding requirements for its SD card, beyond the 
[requirements for a Raspberry Pi](https://www.raspberrypi.org/documentation/installation/sd-cards.md).
Any card with that meets these requirements and is at least 4 GB in capacity will be fine.

1. LED Lights

    These are the most expensive single component in {{ site.name }}, but fortunately you have a lot of options here. I bought
 [this](https://www.adafruit.com/products/2240). The important thing is to buy lights with an APA102C controller.
Many cheaper LED light strips have other controllers with more demanding timing requirements that can
be difficult for a Raspberry Pi to consistently meet.
Adafruit sells the same type of lights in 30 LED/m and 144 LED/m variants and you can get equivalent lights from a variety
of other sources. Make sure you get long enough strips of lights to go around the edge of your TV. Adafruit sells
these lights in one meter lengths, so my 52" TV required purchasing 4 meters of lights to cover.

1. JST Connectors

    JST connectors are used to connect the lights to the Raspberry Pi for data and power. They are also used to join the light
strips on different sides of the TV in later steps. APA102C lights have 4 pins (2 data, 2 power) to connect, so 4 pin JST
connectors like [these](https://www.adafruit.com/products/578) are ideal. Depending on how many lights you have, it's useful
to be able to inject power at the end of the strip or possibly in the middle. 2 pin connectors like [these](https://www.adafruit.com/products/2880)
work well for that. For phase 1, you only need one 4 pin connector and one 2 pin connect, but you can save time by buying more now.
The recommended light strip placement calls for:

    1. Data + power (4 pins) at the start of the strip
    1. 4 joints (2 + 2 pins) between light strips (one in each corner). These joints use two separate connectors to allow
    for the possibility of splicing in power mid-strip if needed for even lighting.
    1. Power (2 pins) at the end of the strip

    In total, this is 1 4 pin connector set and 9 2 pin connectors.
There's also no harm in using connectors for more wires than you need or replacing 4 pin connectors with smaller ones if that's more convenient.

1. [A hat](https://www.adafruit.com/products/2310)

    This is where most of the below components will get soldered into. You can substitute this for any other prototyping board that you can get to plug into the Raspberry Pi's GPIO pins if you want.

