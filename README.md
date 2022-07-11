## Overview
This board uses [ai03's Unified Daughterboard](https://github.com/ai03-2725/Unified-Daughterboard) schematic design but with minor changes. The board is meant to be used in combination with my [Mech-Eighty](https://github.com/rothman5/mech-eighty) keyboard. It's purpose is to provide USB 2.0 full-speed operation circuitry on an external board. It integrates a USB Type C connector and the supporting components onto a small board. The assembly and design of the main keyboard is greatly simplified as a result.


## Features
- Overvoltage and ESD protection on USB voltage supply using a TVS diode.
- Overcurrent protection on USB current supply through a poly fuse.
- Achieves ESD protection on USB data lines using a specialized IC.
> Protection against ESD (electrostatic discharge) surges on the USB data lines is improved using the USBLC6-2SC6 integrated circuit. A single line TVS diode is used to protect the VBUS power line against ESD transients. These devices were chosen to comply with ST's application note ([AN4879](https://www.st.com/resource/en/application_note/an4879-usb-hardware-and-pcb-guidelines-using-stm32-mcus-stmicroelectronics.pdf)) recommendations.
- Noise decoupling with a ferrite bead.
> The ferrite bead inductor represents a low impedance path between the power and signal grounds. High frequency signals experience high impedance because of the bead. This protects against noisy signals passing to the signal ground.
- Shielding capabilities through single path grounding to a metallic case.
- See [ai03's Unified Daughterboard](https://github.com/ai03-2725/Unified-Daughterboard) for more technical information. 


## Photos
![alt text](https://github.com/rothman5/usbc-daughter-board/blob/e23a5fce51890610b72a5b0f3143a3a9a6484dd7/images/front.png)
![alt text](https://github.com/rothman5/usbc-daughter-board/blob/e23a5fce51890610b72a5b0f3143a3a9a6484dd7/images/back.png)


## References
- ST USB power delivery application note ([TA0357](https://www.st.com/resource/en/technical_article/dm00496853-overview-of-usb-type-c-and-power-delivery-technologies-stmicroelectronics.pdf))
- ST USB hardware application note ([AN4879](https://www.st.com/resource/en/application_note/an4879-usb-hardware-and-pcb-guidelines-using-stm32-mcus-stmicroelectronics.pdf))
- ai03's [Unified Daughterboard](https://github.com/ai03-2725/Unified-Daughterboard)
