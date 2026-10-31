# Power Budget

## Overview

This power budget checks that the selected regulator and power supply can power every major component in my light-sensor subsystem at the same time, with a 25% safety margin. It follows the class power budget template.

<img width="735" height="657" alt="image" src="https://github.com/user-attachments/assets/de81cafd-64bf-4bb2-b91d-96df217dc6ad" />


## Summary

| Item | Value |
|---|---|
| Power rails | One 5V regulated rail |
| Total current on 5V rail (with 25% margin) | 42 mA |
| 5V regulator | STMicroelectronics L7805ABV, 1500 mA. **1458 mA remaining** |
| External power source | BestCH 9V 3A wall adapter (EA10302 replacement), 3000 mA. **2952 mA remaining** |
| Battery life | Not applicable (wall supply) |



## Power Budget Calculations
- **Curiosity Nano**: 13.8 × (5/3) + 0.82 = 23.8 mA. Estimated MCU and ADC current; actual 5V board consumption should be verified.
- **MCP6004 Op-Amp**: 0.17 mA × 4 = 0.68 mA. Includes all four amplifiers.
- **Sensor Dividers**: [5V ÷ (0.12 kΩ + 10 kΩ)] × 3 = 1.48 mA. All three photoresistors in direct light.
- Buttons: (5V ÷ 10 kΩ) × 2 = 1.0 mA. Both pressed.
- LEDs: (5 − 3.0)/1 kΩ + (5 − 2.1)/1 kΩ = 4.9 mA. Both on.
- J3 Signal Lines: [5V ÷ (330 Ω + 10 kΩ)] × 3 = 1.45 mA. All three high; motor and driver are in the teammate's budget.
- **Total 5V Current**: 23.8 + 0.68 + 1.48 + 1.0 + 4.9 + 1.45 = 33.33 mA. Estimated load.
- 25% Safety Margin: 33.33 × 1.25 = 41.67 mA. Allowance for variations.
- 9V Supply Current: 41.67 + 6 = 47.67 mA. Includes assumed maximum 7805 quiescent current.
- Regulator Heat: (9 − 5) × 0.04167 + 9 × 0.006 = 0.22 W. About 11°C rise at an assumed 50°C/W junction-to-ambient thermal resistance.
- Regulator Headroom: 9 − 5 = 4V. Above the assumed 2V dropout requirement.
- Battery Comparison: 600 mAh ÷ 47.67 mA = 12.6 hours. Idealized estimate; wall power selected for continuous operation.
Power Configuration: The 9V/3A adapter feeds the L7805ABV regulator, which supplies the 5V rail for the Curiosity Nano and PCB components. The 1A fuse provides fault protection.

## Resouces

The power budget as a PDF download is available [*here*](Powerbudget_304.pdf), and a Microsoft Excel Sheet [*here*](304_pet_feeder_power_budget.xlsx).
