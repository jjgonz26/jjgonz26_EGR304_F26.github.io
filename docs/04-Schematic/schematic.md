---
title: Schematic
---

## Overview

This schematic represents the light sensor system for our automatic pet feeder. The design uses a PIC18F57Q43 Curiosity Nano microcontroller to monitor three photoresistors that detect dfferent food levels. An op amp buffers the sensor signal before they reach the microcontroller. There is also two push buttons for selecting the desired fill level, two indicator LEDs, and an output that will be sent to the motor board and tell it when to activate and when to stop adding food. The board can be powered using a 9V DC input with a voltage regultor or an external regulated 5V supply. There are also additonal GPIO connections for testing and potential troubleshooting.

**Figure 1:** Automated Pet Feeder Light Sensor Schematic

<img width="944" height="944" alt="image" src="https://github.com/user-attachments/assets/a2482052-8d5a-4a8e-8c0a-a1b0e1beb893" />




## Resouces

The schematic as a PDF download is available [here](./JJG_pet_feeder_schematic_v2.pdf), and the Zip folder of the project [*here*](JJG_Pet_Feeder.zip).
