---
title: Schematic
---

## Overview

This schematic represents the light sensor system for our automatic pet feeder. The design uses a PIC18F57Q43 Curiosity Nano microcontroller to monitor three photoresistors that detect different food levels. An MCP6004 operational amplifier(op-amps) buffers the sensor signal before they reach the microcontroller. There are also two push-button switches for selecting the desired fill level, two indicator LEDs, and an output that will be sent to the motor board and tell it when to activate and when to stop adding food. The board can be powered using a 9V DC input with a voltage regulator which will be regulated to 5V or an external regulated 5V supply. There are also additional GPIO connections for testing and potential troubleshooting. The design includes two alternative 8-contact ribbon cable connectors to provide an alternative connection option to J3. And because only one digital signal is needed pins 3 and 5 are just alternate pins available on J3 in case there is issues with pin 4. Also included will be spare GPIO connections where there will be headers in case I run into issues with sensors GPIO's. The LED's and pushbuttons can also be utilized for debugging.

**Figure 1:** Automated Pet Feeder Light Sensor Schematic

<img width="918" height="920" alt="image" src="https://github.com/user-attachments/assets/bec98b6e-1839-44f6-a5f4-dd17b9d3a58a" />





## Resources

The schematic as a PDF download is available [here](./JJG_Sensor_Design_Review.pdf), and the Zip folder of the project [*here*](JJG_Pet_Feeder.zip).
