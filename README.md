# RF_R1_8-9Xu

Open source universal PCB for the Realforce R1 family of keyboards.

## Introduction

This project is a continuation of my development of open source EC boards.

The supported layouts are the one of the Realforce R1 family of keyboards, it being ANSI, ISO or JIS.

## Technical information

- Layout size: tenkeykess (TKL)
- Compatible switches: EC switches (Topre and NIZ)
- Microcontroller: STM32F401
- Connector:
    * internal USB-C
    * original JST connector S4B-EH(LF)(SN)
    * jst connector for daughterboard
- Addressable RGB strip support
- Firmware compatibility: QMK (with VIA/VIAL support)
- Protection hardware (on all connection methods):
  * Fused
  * ESD protection

## Renders and Prototypes

### Render

![PCB Front Render](/Assets/PCB_render_front.png)

![PCB Back Render](/Assets/PCB_render_back.png)

### Prototype

![PCB Front Proto](/Assets/PCB_proto_front.png)

![PCB Back Proto](/Assets/PCB_proto_back.png)

## Revisions and relative features

### Rev1

This revision implements all the main features of the PCB.

#### Connectivity

![Connectivity](/Assets/Connectivity.png)

Since this is first and foremost a replacement PCB for the original Realforce R1 PCB, the original JST connector is still supported. It's been moved to the right to accommodate the new JST connector for the daughterboard and the USB-C connector.

I thought about adding extra connectors so that if anyone wants to use this PCB in a custom project they can have the flexibility to use the connector that they prefer.

#### Addressable RGB strip support

![Connectivity](/Assets/RGB_Strip_Connector.png)

Since the R1 PCB is used in some already existing custom PC (polycarbonate) cases, it was important to have a way to include a RGB strip support.

The strip can be directly sticked to the PCB and then wired to the PCB by soldering the pins to the THT pins or SMD pads.

Lighting can be controlled by the board itself and customization is achieved by using Vial/VIA.

### Rev 1.1

This revision implements the following changes:
  * added support for THT LED for Caps Lock and Scroll Lock
  * moved filtering components for plate shield to top side
  * added filtering components for USB-C shield
  * improved ground stitching

![PCB Front Render Rev 1.1](/Assets/PCB_render_front_1_1.png)

## "Why no plates?" I hear you say

It is what it is.

![walky](https://i.imgur.com/2NHfVwc.gif)

For real though, the PCB is a replacement for the original Realforce R1 PCB so using the original plates is the preferred option. Furthermore, the multilayout support makes it tedious to make a plate design for each and every layout.

Nevertheless, if there's a particular plate config you want to use, you can always open an issue on the repository or even better make a PR from your own fork.

## License

<a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by-nc-sa/4.0/88x31.png" /></a><br />This work is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by-nc-sa/4.0/">Creative Commons Attribution-NonCommercial-ShareAlike 4.0 International License</a>.
