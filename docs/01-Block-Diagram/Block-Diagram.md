---
title: Individual Block Diagram
tags:
- tag1
- tag2
---

## Overview
The block diagram below demonstrates the measuring and control subsystem for Team 206's pet feeder. It shows the connections between the three light sensors, push buttons, LEDs, curoisty nano board, power supply, and team interface, including signal types, voltagle levels and pin assignment.

## Power Source
The subsystem is powered from 9 V, 3 A unregulated supply. The 9V supply feeds a voltage regulator that provides a regulated 5 V output for the subsystem.

## Power Levels
The PIC18F57Q43 Curiosity Nano and MCP6004 op-amp operate using the regulated 5V supply. The photoresistor voltage dividers, push-button circuits, and LEDs also operate within the 0-5V range. The 9V supply provides the input to the 5V voltage regulator.

## Sensors
Each photoresistor forms a voltage divider that produces an analog signal. The signal is filtered and buffered using an MCP6004 op-amp configured as a voltage follower before being read by the PIC18F57Q43 ADC

## Actuators/ Outputs
Two LEDS provide visual indication of the selected fill level. The microcontroller also provides digital output signal to the motor subsystem when filling should begin or stop based on the selected level and sensor reading.

## Team Connections:
This board will be connected to AJ's board to give an input to control the motor. On my individual board I will have two options for connectors one will have 3 potential pin connections the other will only have the one. They are all potential options for the same individual digital signal that will be sent to AJ's board to be the motor control signal.

| Ribbon Pin J3 |Direction |My MCU Pin |Purpose|   
|---|---|---|---|
|1-2|-|-|Unused|
|3,4,5| Justin → AJ| RC2| Motor/Fill control signal|
|7|-|-|Unused|
|8|-|GND|Shared ground|

| Ribbon Pin J5 |Direction |My MCU Pin |Purpose|   
|---|---|---|---|
|1-3|-|-|Unused|
|4| Justin → AJ| RC2| Motor/Fill control signal|
|5-7|-|-|Unused|
|8|-|GND|Shared ground|


## Justin Gonzalez Block Diagram 
[Link to individual .drawio](https://drive.google.com/file/d/1Y3qVkam38sxITZQeANNHaddejhfWaVvK/view?usp=sharing)

<img width="1112" height="1121" alt="304 Individual block diagram 206  drawio (3)" src="https://github.com/user-attachments/assets/6117f8c1-6941-4f08-b233-0e031974287c" />


