---
title: BAMFK-1 Build Guide
---

:::info

This guide is currently a work in progress, and a full write-up is in the works.

:::

## Parts List

* [Big Switch](https://novelkeys.com/products/the-big-switch-series)
* [BAMFK-1 Acrylic Case](https://keeb.io/products/bamfk-1-acrylic-case-for-big-switch)
  * Note: If you've purchased this kit, you will have the rest of the parts below
* [BAMFK-1 PCB](https://keeb.io/products/bamfk-1-big-switch-pcb)
* EC11B Horizontal Encoders
* Encoder Knobs
* 1.5mm and 2.5mm Hex Keys
* M3 screws and rivet nuts

## Build Steps Summary

1. Remove top half of case
2. Insert switch into plate
3. Solder encoders
4. Install knobs
5. Solder Big Switch
6. Insert plate into case
7. Reassemble top half of case

## Remove Top Half of Case

:::info

If your case has been fully disassembled, you'll need to reassemble the bottom portion of the case first. See the steps for [making the bottom half](#make-bottom-half-of-case) first before following the rest of these steps.

:::

Unscrew the screws at the top of the case and remove the top layers and switch plate. Don't unscrew the bottom portion of the case and leave it as is.

## Insert Switch into Plate

Insert the Big Switch into the switch plate, making sure the holes are in the correct orientation as shown below.

## Solder Encoders

Solder the rotary encoders to the PCB.

:::warning

Make sure you insert the encoders from the bottom side of the PCB and solder them in place on the top side. You may have a hard time desoldering the encoders if you inserted them on the wrong side.

:::

## Install Knobs

Install the knobs onto the rotary encoders and use the 1.5mm hex key to tighten them into place. It'll be more difficult if you screw on the knobs later, so do it now.

## Solder Big Switch

Insert the switch legs of the Big Switch through the PCB and solder them on. You may find that you need a decent amount of solder to get everything in place. If you don't use enough solder, the PCB might hang off of the switch at an angle.

## Insert Plate into Case

Take the plate/PCB/switch combo and angle in the knobs through the front panel first, and then lean the USB port back.

## Reassemble Top Half of Case

Reassemble the top half of the case as described here: [Making Top Half of Case](#make-top-half-of-case).

## Reprogramming the BAMFK-1

You can reprogram the BAMFK-1 using QMK, QMK Configurator, or VIA Configurator. The encoder rotations and presses can be programmed as well.

### QMK Configurator

Here's the link for configuring the BAMFK-1 with QMK Configurator: <https://config.qmk.fm/#/keebio/bamfk1/LAYOUT>

![](./assets/images/bamfk-1/bamfk-qmk-config.png)

### VIA Configurator

Since the [pull request for VIA support of the BAMFK-1](https://github.com/the-via/keyboards/pull/1211) is still pending, you will have to manually load in the `bamfk1-rev1.json` file everytime you launch VIA so that your board can be detected.

Here's the steps for setting this up:

#### Initial Setup

You will only need to go through the following steps once:

1. Download this VIA .json file: [BAMFK-1 VIA JSON](https://raw.githubusercontent.com/nooges/via-keyboards/bamfk-1/src/keebio/bamfk1/bamfk1-rev1.json).
2. Open up VIA and go to Setting tab, enable `Show Design tab`

![](./assets/images/via/enable-design-tab.png)

#### Loading in Definition File

Each time you launch VIA, you will need to load in the BAMFK-1 definition file downloaded earlier

1. Go to Design tab and load in the `bamfk1-rev1.json` file (you will need to do this each time you launch VIA)

![](./assets/images/via/load-draft-definition.png)

![](./assets/images/bamfk-1/bamfk-via-config.png)

## Full Reassembly of Case

If you've completely disassembled the case, here's how to put all the pieces back together.

First you'll need to identify all of the pieces. Each piece has a number of registration dots to assist with identification and placement, since some of the layers are similar in size.

The registration dots are aligned towards the left side of the case, except for the layers that come in two pieces (and thus will have dots on both the left and right sides).

### Make Bottom Half of Case

We are going to assemble the case, starting from the bottom plate.

Make sure the registration dot is aligned to the left. Then add rivet nuts on the underside of the plate in the spots indicated below.

![](./assets/images/bamfk-1/b7.png)

Find the piece with 2 dots and stack it on top of the bottom plate.

![](./assets/images/bamfk-1/b6.png)

Do the same with the piece with 3 dots.

![](./assets/images/bamfk-1/b5.png)

There will be two pieces with 4 dots.

![](./assets/images/bamfk-1/b4.png)

Then put on the two pieces with 5 dots.

![](./assets/images/bamfk-1/b3.png)

Add the piece with 6 dots.

![](./assets/images/bamfk-1/b2.png)

Add the piece with 7 dots.

![](./assets/images/bamfk-1/b1.png)

Insert the front panel piece, making sure the registration dot is aligned to the top left.

![](./assets/images/bamfk-1/fp.png)

Take the 35mm M3 screws and slot them through all the pieces stacked so far and screw them into the rivet nuts.

![](./assets/images/bamfk-1/rivets1.png)

### Make Top Half of Case

Add the switch plate.

![](./assets/images/bamfk-1/sp.png)

Add the piece with 2 dots.

![](./assets/images/bamfk-1/t1.png)

Add the piece with 1 dot.

![](./assets/images/bamfk-1/t2.png)

The last three pieces are all the same size and have no dots.

![](./assets/images/bamfk-1/t3-5.png)

Add the remaining rivet nuts to the bottom plate and screw in the 70mm M3 screws into them.

![](./assets/images/bamfk-1/rivets2.png)