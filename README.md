# VR Ambilight (WORK IN PROGRESS)
## Introduction

The VR Ambilight is a project that enhances the immersive experience of virtual reality (VR) by creating dynamic ambient lighting that synchronizes with the on-screen content. This guide will walk you through the process of building your own VR Ambilight system.

Features

    Dynamic ambient lighting synchronized with VR content.
    Adjustable color and brightness settings.
    Support for Valve Index.

## Materials

Before you begin, make sure you have the following materials:

    Arduino Nano.
    WS2812b Individually Addressable led Strip 144Pixels/m.
    Soldering equipment.
    Defusion sheet (recomended)

## Wiring Diagram
Follow this wiring diagram to connect the components correctly:

Ensure that the LED strip you are using operates at a voltage of **5V**.
![Wiring.jpg](https://github.com/Statonwest/VR_Ambilight/blob/01b49622970872a12339bb632445c691a10369d1/Wiring%20Digram.jpg)
Typically, for larger LED strip setups, you would require a separate power supply unit (PSU). However, in this case, the number of LEDs is small enough to be powered directly from the Arduino board itself.

## Arduino Setup

To set up the software, follow these steps:

Download and install the Arduino IDE from the official Arduino website (https://www.arduino.cc/en/software).

Install the [FastLED libruary](https://github.com/FastLED/FastLED/releases).

Clone or download the project files from the GitHub repository:
[VR_Ambient_light.ino](https://github.com/Statonwest/VR_Ambilight/blob/4264298c710a5be8f2513a294410e2fc3ae0b779/VR_Ambient_light.ino)

The original repository can be found here.
[adalight.ino](https://github.com/hyperion-project/hyperion.ng/blob/master/assets/firmware/arduino/adalight/adalight.ino)

## Building the VR Ambilight

Follow these steps to assemble the VR Ambilight system:

Cut two LED strips with 9 LEDs each.

Solder the two indoviual strips together with lenghs of wire long enough to rout around to each side of the face gasket.

Connect the data line, GND, and the 5V of the LED strip to the Arduino. Connect the DIN (data input) pin of the LED strip to digital pin 6.

Double-check all the connections and make sure they are secure.

Position the LED strip around the perimeter of your face gasket, ensuring an even distribution of light.

I chose to route my wires from underneath and over the top of the gasket. There are many ways to arange them with the same result. Just be sure to adjust your Prismatik settings accordingly.
###ADD PIC HERE###

Cut out the defusion sheet accroding to the template [Diffusion Template](https://github.com/Statonwest/VR_Ambilight/blob/4022c5608829f168b4be608d5043e20a68479a2e/Diffusion%20Template.pdf). The deffusion sheet I used was from an old display. But parchment paper can work in a pinch.
I used 2 polorizing layers and the top diffusion sheet.
###ADD PIC HERE###

###Add section about how arduino is mounted###

## Prismatik

[Prismatik](https://github.com/psieg/Lightpack/releases) 
is what we will use to capture the screen and send the data to the arduino.
##add more here##

Adjust the color and brightness settings according to your preference in Prismatik.
##add more here##
