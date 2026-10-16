---
title: Component Selection
---

**Table 1: Op Amp**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
|<img width="200" height="200" alt="MCP6004" src="https://github.com/user-attachments/assets/6a7ad8c6-ad99-470a-b112-e7f20242e0b2" /> <br>\* Option 1.<br>\* MCP6004-I/P Quad Operational Amplifier<br>\* $0.60/each<br>\*[Link to product](https://www.digikey.com/en/products/detail/microchip-technology/MCP6004-I-P/523060)                 | \* Operates on 5V<br>\* Four amplifiers in one<br>\* Low supply current (100 μA per amplifier)<br>\* Rail-to-rail inputs and outputs                                               | \* Maximum Supply Voltage 6V needs regulation from 9V power source <br>\* Lower bandwidth (1 MHz) than the TL974IN (12 MHz)<br>\*Input offset voltage can introduce small measurements errors |
| <img width="200" height="200" alt="TL974IN" src="https://github.com/user-attachments/assets/c6fdefa1-d144-4de3-8a11-81a5f1e29387" /> <br>\* Option 2. <br>\* TL974IN Quad Operational Amplifier <br>\* $1.66/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/texas-instruments/TL974IN/1675406) | \* Works with 5V supply<br>\* Four amplifiers in one <br> \* Higher bandwidth(12 MHz) | * More expensive <br>\* Higher power consumption <br>\*Limited input common mode voltage range                                                       |
|<img width="200" height="200" alt="LM324N" src="https://github.com/user-attachments/assets/3b57f81f-bab1-4d46-a6dc-1afbfa9414f0" /> <br>\* Option 3. <br>\* LM324N Quad Operational Amplifier <br>\* $0.58/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/texas-instruments/LM324N/277627) | \* Operates on 5V<br>\* Four amplifiers in one <br> \* Inexpensive | * Not rail-to-rail <br>\* Input common-mode range does not extend to the positive 5V supply rail <br>\*Higher input bias current (45nA) than the MCP6004 (1pA)                                                       |

**Choice:** Option 1:  MCP6004-I/P Quad Operational Amplifier

**Rationale:**

<br>
<br>

**Table 2: Light Sensor**

| **Solution**                                                                                                                                                                                      | **Pros**                                                                                                                                    | **Cons**                                                                                            |
| ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- | --------------------------------------------------------------------------------------------------- |
|<img width="200" height="200" alt="PDV-P8103" src="https://github.com/user-attachments/assets/7b3fc928-6784-40d7-aba1-716108db69dc" /> <br>\* Option 1.<br>\* PDV-P8103 CdS Photoresistor <br>\* $0.72/each<br>\*[Link to product](https://www.digikey.com/en/products/detail/advanced-photonix/PDV-P8103/480610)  | \* Inexpensive<br>\* High dark resistance (500 kOhms minimum)<br>\* Resistance changes with light exposure                                               | \* Requires a voltage-divider circuit <br>\* Lower minimum dark resistance than option 2<br>\*Ambient Lighting may affect readings |
|<img width="200" height="200" alt="NSL-A95013" src="https://github.com/user-attachments/assets/afd7d758-f4bd-4232-9bcf-e6b3622b88fb" /> <br>\* Option 2. <br>\* NSL-A95013 CdS Photoresistor <br>\* $0.88/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/advanced-photonix/NSL-A95013/26316781) | \* High minimum dark resistance (1.2 MOhms)<br>\* Resistance changes with light exposure <br> \* Good at detecting blocked light | * More expensive than Option 1<br>\* requires a voltage divider circuit <br>\*Ambient lighting may affect readings                                                       |
|<img width="200" height="200" alt="161 CDS Photoresistor" src="https://github.com/user-attachments/assets/56e7dd68-b44c-449e-bd7f-2722f7d5b93c" /><br>\* Option 3. <br>\* Adafruit 161 CdS Photoresistor <br>\* $0.95/each <br>\* [Link to product](https://www.digikey.com/en/products/detail/adafruit-industries-llc/161/7244927?s=N4IgTCBcDaIAQEEAmBDAZgJwK4EsAucAjAGyFwDCSAynAAoAWA9noxgKYDOOHLGIAugF8gA) | \* Simple design<br>\* Through hole installation<br> \* Detects changes in light when sensor is blocked| * Most Expensive<br>\* Low Minimum dark resistance (200 kOhms) <br>\*Light resistance is not listed                                                    |

**Choice:** Option 1:  

**Rationale:**
