# [Air Quality]

<!-- Project Banner / Board 3D Render Image -->
![Project Render](docs/images/board_render.png)

## Overview
- **Description:** STM32 based custom-board to monitor temperature, humidity and VOC
- **Status:** Revision 1.0
- **License:** Apache-2.0 license

## Description
Me and my fellow contributors were looking for a nice embedded project to have some fun. One of us was arguing about having a terrible air quality in its bedroom and... Here we are.

## Key Features
- LCD TFT [dimension] Display
- Dimmable display backlight
- USB-C powered (5V)
- ...

## Technical Specifications
| Parameter | Value |
| :--- | :--- |
| **Input Voltage** | 5V |
| **Microcontroller / Core** | STM32L431CCT6TR |
| **Dimensions** | 60x40 mm |
| **PCB Layers** | 2 |
| **...** | ... |


## Project Structure (TODO)
```text
├── docs/             # Documentation, schematics PDF, and renders
├── fabrication/      # Production files (Gerbers, BOM, Pick & Place)
├── design/           # KiCad project source files
│   └── .../         # ...
├── exported            # .step, BOM, ...
├── LICENSE           # License file
└── README.md         # Project documentation
```

## Hardware Documentation (TODO)
- **Schematic (PDF):** [Link to Schematic PDF](docs/schematic.pdf)
- **Interactive BOM:** [Link to ibom.html](docs/ibom.html)
- **Design Software:** KiCad 10.0

### Pinout & Connectors
For the complete pinout, look after the schematic.
| Pin | Function | Description | Direction
| :--- | :--- | :--- | :--- |
| PA1 | SPI_CLK | SPI Clock Signal | Out |
| PA3 | BUTTON_IN | External Button Signal | In |
| PA4 | DC_DISPLAY | | |
| PA5 | RST_DISPLAY | | |
| PA6 | CS_DISPLAY | | |
| PA7 | SPI_MOSI | | |
| PA8 | BCK_LIGHT_DISPLAY | Display Backlight Signal | Out |
| PA9 | I2C_SCL | SCL Line of I2C bus | Out |
| PA10 | I2C_SDA | SDA Line of I2C bus | In / Out |
| PA11 | SWDIO | | |
| PA14 | SWCLK | | |
| PB3 | SWO | | |


## Ordering & Fabrication Guidelines (TODO)
The chosen manufacturer is AISLER and every constraints in the layout that I used is based on their specifications.
- **PCB Thickness:** 1.6 mm
- **Layers:** 2
- **Surface Finish:** HASL / ENIG
- **Copper Weight:** 1 oz
- **Min Trace / Space:**


## Test Firmware
The test firmware written in C is provided at: TODO <br>
More information about it are provided in the linked repository.

## Revision History
- **v1.0:** First working prototype

## Project Constraints and Limitations
Given the fact that this is an hobbistic project and not a lot of time could have been spent on it, those are some of the decisions that we took:
- We like display and embedded graphics, so an RGB display is a must have
- We want to produce a complete product (with a plastic case, etc..) so it be as simple as possible
- I'm not an professional hardware designer (firmware guy btw) so the electronics on the PCB should be "mainstream"
- It MUST be as cheap as possible (and so the component and feature selection) given the tight budget I assigned on that project
- It's goal is to be placed on a desk as a gadget (and not a professional HVAC device)

## License
Distributed under the Apache-2.0 License. See `LICENSE` for more information.

## Contributing & Support
I would like to thanks my friends which worked on the final firmware product and device enclouse:
- ...
- ...
- ...