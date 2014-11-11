---
layout: post
title: How We Build Prototypes Fast
author: Andrew Madsen
author_twitter: armadsen
Category: Hardware
---

As I’ve been working on the design of the Bluetooth electronics, I thought it would be worth explaining a little about the early stages of the hardware prototyping, the choices we’re making, and what impact they will have on the final product.

The first step in any hardware project is to create a 'bread board' prototype. This is where the real design of the hardware begins. Usually, this means assembling everything by hand in a way that it can be easily modified and added to as the design evolves. In modern hardware projects, where firmware is as or even more important than the hardware itself, it's helpful if your prototype is easily programmable.

Even before we started prototyping the Wired In Bluetooth electronics, we had a lot of decisions to make: Exactly what capabilities does the hardware need to have? How will it be powered? Batteries, USB, or both? Are we just trying to prove out the concept or actually start designing the hardware we intend to put in the finished signs? We discussed all of these. For our first prototypes, we’re most concerned with the ability to communicate with a sign over Bluetooth from a Mac or iOS app. We wanted the ability to turn the light on and off, and to control the color of its LEDs. This will allow us to start developing real software while we continue to refine our hardware designs.

![RFDuino and USB Shield]({{site.url}}/assets/rfduino_and_dev_usb_shields.jpg)

For our prototype phase, we've chosen to use an [Arduino](http://arduino.cc), more specifically an [RFDuino](http://www.rfduino.com). We get a number of advantages out of this. The Arduino was created from the beginning to be very easy to get up and running quickly without a lot of overhead. This is an advantage when you’re new to microcontrollers, but the same things that make it easy for beginners also make it really attractive as a prototyping platform.

At this point, there’s a large community around the Arduino. There are lots of available resources, including: tutorials, documentation, open source hardware designs, and perhaps most importantly, software libraries. The RFDuino comes with a library of functions that makes communicating via Bluetooth 4.0 very easy. If we were to use our own microcontroller and Bluetooth transceiver combo, we might end up needing write the low level communications routine that allow the microcontroller to talk to the transceiver.

Arduino hardware is also modular. For prototyping, we’re using an RFDuino, which includes Bluetooth 4.0 capability, a USB shield to allow wired power and communications, and a RGB module which includes buttons and an RGB LED much like those we’ll be using in the production Wired In signs. These modules all plug together without us having to do any wiring. There are a number of other shields available in case we need additional functionality or want to experiment with other features. All of this allows us to start immediately focusing on the overall design, and especially the firmware without a lot of fussing around.

![RFDuino, RGB, and Battery Shields]({{site.url}}/assets/rfduino_and_rgb_led_and_battery_shields.jpg)

It turns out that the Arduino can also work well in production devices. We’re still discussing and deciding whether we’ll use an Arduino in the final product or move to using lower level discrete parts. Using discrete parts will reduce the per-unit manufacturing cost and gives us more flexibility, but will make for longer engineering time. In the prototyping phase, where cost is not a big concern, and where we mostly just want everything to work, using an Arduino is a big win.

-Andrew
[@armadsen](http://twitter.com/armadsen)