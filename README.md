# QMX+ Battery & Audio Board

This project is a custom battery and audio module designed for the QRP-Labs QMX+ transceiver. The module is designed to be directly mounted on the existing circuitry inside the QMX+ for seamless integration. 

## Features
- Integrated battery power supply
- Built-in audio amplifier
- Direct mounting on QMX+ PCB
- Easy to assemble and efficient design

## Images

![Assembled Front](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembled%20Front.jpeg)

![Assembled Front With Speaker](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembled%20Front%20with%20Speaker.jpeg)

![Assembled Top](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembled%20Top.jpeg)

![Assembled Back Without Top Cover](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembled%20Back%20Without%20Top%20Cover.jpeg)

![Assembled Back With Top Cover](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembled%20Back%20With%20Top%20Cover.jpeg)

![Schematic](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/QMX%2B%20Battery%20%2B%20Audio%20Board%20Rev.%201.1%20Schematic.jpg)

![3D Front](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Rev.%201.1%203D%20Front.jpg)

![3D Back](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Rev%201.1%203D%20Back.jpg)

## Required Components
- **3x 18650 Li-ion Batteries:**
- **1x 3S 20A BMS Board** 
- **1x LM386 Audio Amplifier Breakout Board:** Easy to assemble breakout board.
- **1x 3A Fuse:** For further protection.
- **1x Fuse Holder:**
- **2x 1K 1/4W THT or 0805 SMD Resistors:** Solder as you like SMD or THT.
- **8 Ohm Speaker:** Necessary for audio output. Use the screw terminals on the audio amplifier board.
- **1x 2x3, 1x 2x2, 1x 1x5 2.54mm Female and Male Pin Headers:** To mount the pcb directly on the main board.

### Used Modules

| 3S 1A Multi Cell Charger Board | LM386 Audio Amplifier Breakout Board | 3S 20A BMS |
|---------|---------|---------|
| ![3S 1A Multicell Charger Board](Images/3S%201A%20Multicell%20Charger%20Board.jpg) | ![LM386 Audio Amplifier Breakout Board](Images/LM386%20Breakout%20Board.jpg) | ![3S 20A BMS](Images/3S%2020A%20BMS.jpeg) |

## Assembly and Calibration

### Assembly

Assembly order is not important. Resistors can be 1206 SMD or 1/4 W THT. Solder as you like. 

You must give attention to positive and negative terminals indicators of your battery holders to lower the chance of accidents. 

You must change the orientation of the original headers found on audio amplifier board.

Modules should be soldered on top of single header pins just like in the photo above.

To solder the radio connection headers, it is advised to solder the QMX+'s headers first. Place the board on top of the mainboard of QMX+ with suitable headers, connect the boards with screws and then solder the headers to the battery board. This ensures our board lies flat on top of the mainboard.

You should mark and drill the back plate after you screw the board to the mainboard. Board must be flat and sturdy.

**When all components are soldered you should test and inspect your board with a multimeter according to the schematic. If you are sure about it then insert the batterries correctly and power it on.**   

![Assembling Modules](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembling%20Modules.jpeg)

### Audio Calibration

After assembly and testing that your radio works you must calibrate the audio.

To calibrate the audio you must first lower the volume as down as you can using the volume knob of the radio. Then you must turn the variable resistor found on the audio board until you can hear the audio coming from the speaker barely. Audio is calibrated you should use the volume knob from now on.

**Note : Images above include *Rev. 1* which is the prototype version of this board. Assembly guide is identical to the *Rev. 1.1* The main difference between these revisions is switch option to change between charge and operation mode which is found unnecessary during testing. Minor silkscreen changes and footprint changes also made.**