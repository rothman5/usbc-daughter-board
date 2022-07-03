# Daughter Board
This board is meant to be used in combination with my [Mech-Eighty](https://github.com/rothman5/mech-eighty) keyboard. 
It's purpose is to provide USB 2.0 full-speed operation circuitry on an external board.
It integrates a standard USB Type C connector and the supporting components onto a small board.
The assembly and design of the main keyboard is greatly simplified as a result.

## Features
- Achieves ESD (electrostatic discharge) protection on USB data lines using a specialized IC.
- Overvoltage protection on USB voltage supply using the same IC.
- Overcurrent protection on USB current supply through a poly fuse.
- (TODO) Single path grounding support.

## Photos
![alt text](https://github.com/rothman5/usbc-daughter-board/blob/c97103dfde8c70be1457c372696d8910cc421555/images/front-preview.png)
![alt text](https://github.com/rothman5/usbc-daughter-board/blob/c97103dfde8c70be1457c372696d8910cc421555/images/back-preview.png)

## References
- ST's [TA0357](https://www.st.com/resource/en/technical_article/dm00496853-overview-of-usb-type-c-and-power-delivery-technologies-stmicroelectronics.pdf) power delivery article
- ai03's [Unified Daughterboard](https://github.com/ai03-2725/Unified-Daughterboard)
