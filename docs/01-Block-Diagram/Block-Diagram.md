---
title: Individual Block Diagram
tags:
- tag1
- tag2
---

## Overview
The block diagram below shows the measuring subsystem for Team 206's pet feeder. It shows how the three light sensors, push buttons, LED, microcontroller pins, power levels, and team connection are arranged. The diagram will be updated with part numbers for design review.

## Power Source
The subsystem is powered from 9 V, 1 A unregulated supply. The 9V supply feeds a voltage regulator that provides a regulated 5 V output for the subsystem.

## Power Levels
The PIC18F57Q43 Curiosity Nano, photoresistor, op-amp, pushbutton and LEDS are all on a 5 V rail. The 9 V rail is used as the input to the 5 V regulator.

## Sensors
The subsystem uses three photoresistors to monitor the food level in the feeder. Photoresistor 1 detects the empty level, Photoresistor 2 detects the low-fill level, and Photoresistor 3 detects the high-fill level. Each sensor signal is conditioned by an op-amp circuit and then read by an ADC input on PIC18F57Q43.

## Actuators/ Outputs
Two LEDS provide visual indication of the selected fill level. The microcontroller also provides digital output signal to the motor subsystem when filling should begin or stop based on the selected level and sensor reading.

## Team Connections:
This board will be connected to AJ's board to give an input to control the motor.

| Ribbon Pin |Direction |My MCU Pin |Purpose|   
|---|---|---|---|
|1-3|-|-|Unused|
|4| Justin → AJ| RC2| Motor/Fill control signal|
|5-7|-|-|Unused|
|8|-|GND|Shared ground|




## Justin Gonzalez Block Diagram 
[Link to individual .drawio](https://drive.google.com/file/d/1Y3qVkam38sxITZQeANNHaddejhfWaVvK/view?usp=sharing)

<img width="922" height="978" alt="304 Individual block diagram m206  drawio" src="https://github.com/user-attachments/assets/76b2101a-3cc6-47f1-8057-180fdf878dfa" />

