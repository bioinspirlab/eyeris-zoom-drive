# EyeRIS Zoom Drive

## Overview
This repo contains the models and associated part to build a remote zoom controller for a Canon 70-200 mm zoom lens. The goal is to enable a relatively simple path to building remote zoom control for DSLR and Mirrorless full frame lenses.

## Components of the Lens Drive
- [Pololu Tic T825 Stepper Motor Controller](https://www.pololu.com/product/3131)
- [Faulhaber DM1220 Stepper Motor](https://www.faulhaber.com/en/products/series/dm1220/)
- [Faulhaber 12 mm, 256:1 Planetary Gear Head](https://www.faulhaber.com/en/products/series/124/)
- [Onedrives.us Spur Gear 48 pitch, 24-tooth](https://www.ondrivesus.com/precision-spur-gears/inch-series/sg48p10a-24)
- [Raspberry Pi3](https://www.raspberrypi.com/products/raspberry-pi-3-model-b/)
- [Stepper Driver Control Software](https://github.com/bioinspirlab/eyeris-camera-control/blob/main/server/libs/zoom_control.py)
- 3D printed parts from the models/assembly subdir

## Using the existing models
The models in this repro should work well with the second generation of the Canon 70-200 mm EF mount zoom lens. The the assemlies subdir, there are STEP and Solidworks files for all of the parts needed to build the zoom drive. The parts were printed on a Multijet Fusion printer and have been tested during many field trials.

## Adapting the models to a new lens
In general, this approach should work well for a range of lenses with manual zoom control. The appropriate motor, spur gear, and 3D printed gear will depend on the diameter of the zoom barrel on the lens and the required torque. This repo includes a TorqueTool part that can br printed to measure the torque needed to activate the zoom lens using a standard socket torque wrench. 
