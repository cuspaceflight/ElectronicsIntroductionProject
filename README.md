# Introduction Project

## Supplied components
- Arduino Nano
- BMP180
- SPDT switch
- Micro SD card reader
- Micro SD card
- PH2.0 battery connector
- 2S LiHV battery (13x17x52mm)

## Constraints
Must fit within a 25mmx120mm Cylinder. This includes both the designed PCB and LiHV battery

## Schematic design Task

1. Add the BMP180, MicroSD card reader, switch and 2 pin connector to the schematic
    The BMP180 and MicroSD card schematic designs are provided in this template and the switch and 2 pin connector are provided by KiCad
2. Add the connections from each component to each other, this will require finding the pinout of the arduino nano to
    correctly wire the MicroSD card and BMP180. The BMP180 uses an I2C interface, while the MicroSD uses SPI.

## Other information
On the launch day we will supply the LiHV batteries, we can also provide these
before hand for testing but we are not able to give them out.

We are aiming for 10 boards to be manufactured due to component count. If more components
are required then we are also able to buy more.

## PCB design Task
Introductory Electronics Project PCB Design

Requirements:
- Total must fit within a 25x120mm cylinder, which needs to include both the designed PCB, as well as the LiHV battery.
- LiHV battery has dimensions: 13x17x52mm.
- Switch footprint: SW_Slide_SPDT_Angled_CK_OS102011MA1Q

Design Tips:
- Think about copper trace layouts – there are 2 copper layers (front and back), which can both be used, try and minimise the number of vias used to switch sides.
- Components can be places on both sides of the board.
- Think about access needed for some components – the Arduino Nano will need to have a microUSB plugged into it for programming, and the SD card will need to be removable, so don’t block the space needed for this.
- When creating the copper traces, don’t have 90° corners, use 45° turns.
- Avoid wrapping traces around component pins, this can lead to interference, and potentially unreliable operation.
- Think about where the components are being placed, since the board needs to be manufactured and assembled – don’t put the pins too close to the edge, and remember you’ll need to solder the components where you’ve placed them.
- Use a ground fill on one side of the board instead of just connecting all the grounds by wire – much more reliable and good design practice. Ensure that ground fills are kept as continuous as possible and only cut through/interrupt them if necessary.
- Run the DRC in the PCB editor once you think you’ve finished and look for things it suggests/flags as an error.
- The design requirements for the boards are an absolute maximum! If you can make the board smaller, then go for it!
