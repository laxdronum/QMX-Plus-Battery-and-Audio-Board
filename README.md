# QMX+ Battery & Audio Board/Shield

This project is a custom battery and audio board designed for the QRP-Labs QMX+ transceiver. The module is designed to be directly mounted on the mainboard of the QMX+. **It is design to work with 12V.**

### Please check my website for latest info about buying one of this board : [Link](https://ta7mna.com/blog/information-about-the-new-batch)

### Next Steps After Assembling or Recieving your Board (Guide): [Link](https://ta7mna.com/blog/next-steps-after-receiving-your-fully-assembled-board-rev-1x)

### Review by Colin MM0OPX (Video): [This SIMPLE Mod Makes the QMX+ Even Better](https://www.youtube.com/watch?v=ZL12OHniudg)

## Features
- Integrated battery power supply
- Designed to work with 12V QMX+ transcievers
- Built-in audio amplifier
- Direct mounting on QMX+ PCB
- Type-C port for charging
- Integrated BMS
- Easy to assemble and efficient design

## Revision History - Last Revision : Rev. 1.2

* March 2025 Rev. 1 : Prototype version. Had a switch option to change between charging and operation mode and battery disengagement didn't work. I fixed the issue by modifying the board. BMS pins were also slightly off due to different revisions of the BMS board.
* April 2025 Rev. 1.1 : First version that I shared on Github. Removed the switch option and battery disengagement issue fixed. BMS pins also fixed and made compatible with all BMS revisions.
* May 2026 Rev. 1.2 : Second version. Some fuse holders were not compatible with Rev. 1.1 due to pin spacing issue. Rev. 1.1 only supported fuse holders with 600mil (15.24mm) pin spacing. Added 900mil (22.86mm) option. 

## Images

![Assembled Front](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembled%20Front.jpeg)

![Assembled Front With Speaker](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembled%20Front%20with%20Speaker.jpeg)

![Assembled Top](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembled%20Top.jpeg)

![Assembled Back Without Top Cover](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembled%20Back%20Without%20Top%20Cover.jpeg)

![Assembled Back With Top Cover](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembled%20Back%20With%20Top%20Cover.jpeg)

![Schematic](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/QMX%2B%20Battery%20%2B%20Audio%20Board%20Rev.%201.2%20Schematic.jpg)

![3D Front](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Rev.%201.2%203D%20Front.jpg)

![3D Back](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Rev%201.2%203D%20Back.jpg)


## Warning and Disclaimer - It is designed to work with 12V version.

## When operating the QMX+, always power off the device before disconnecting the DC power supply. Unplugging the DC jack while the battery board is installed can cause a voltage transient as the battery board takes over, which may lead to damage of the mainboard's voltage regulators.

**I am not responsible for any damage to your equipment, injury, or any other consequences resulting from the use or misuse of this project. Double-check all connections and follow safety guidelines. Build and use this project at your own risk.**

**If you are using the 9V version of the QMX+ and used my board to power it up, you'll likely to fry the PA transistors. You'll have to replace four BS170 found in your QMX+. This board is for 12V version of the QMX+. You can desolder and rewind the PA transformer for 12V.**

**Please do not copy and rebrand my project. You are free to use it with my labels.**

## Required Components
- **3x 1x18650 Li-ion Batteries:** I used 2900mAh INR18650 cells. There must be three 1x18650 battery holders.
- **3S 1A Multi Cell Charger Board (DDTCCRUB):** I used 1A and 2A versions. 3A might be a problem due to heating.
- **1x 3S 20A BMS Board** 
- **1x LM386 Audio Amplifier Breakout Board:** You have to desolder the pins.
- **1x 5x20mm 3A Fuse:** For further protection.
- **1x 5x20mm Fuse Holder:** Compatible with most 2 pin 5x20mm fuse holders. It must have 22.86mm (0.9in) or 15.24mm (0.6in) pin pitch.
- **2x 1K 1/4W THT or 0805 SMD Resistors:** Solder as you like SMD or THT.
- **8 Ohm Speaker:** Necessary for audio output. Use the screw terminals on the audio amplifier board. Small laptop speakers should work.
- **1x 2x3, 1x 2x2, 1x 1x5 2.54mm Female and Male Pin Headers:** To mount the PCB directly on the main board.

### Used Modules

| 3S 1A Multi Cell Charger Board | LM386 Audio Amplifier Breakout Board | 3S 20A BMS |
|---------|---------|---------|
| ![3S 1A Multicell Charger Board](Images/3S%201A%20Multicell%20Charger%20Board.jpg) | ![LM386 Audio Amplifier Breakout Board](Images/LM386%20Breakout%20Board.jpg) | ![3S 20A BMS](Images/3S%2020A%20BMS.jpeg) |

## Assembly, Calibration and Notes

### Assembly

* Assembly order is not important. Resistors can be 0805 SMD or 1/4 W THT. Solder as you like. 

* You must give attention to positive and negative terminals indicators of your battery holders to lower the chance of accidents. 

* You must change the orientation of the original headers found on audio amplifier board.

* **Modules should be soldered on top of single header pins just like in the photo below.**

* **To solder the radio connection headers, it is advised to solder the QMX+'s headers first. Place the board on top of the mainboard of QMX+ with suitable headers, connect the boards with screws and then solder the headers to the battery board. This ensures our board lies flat on top of the mainboard.**

* **You should mark and drill the back plate for type-c port after you screw the board to the mainboard. Board must be flat and sturdy.**

**When all components are soldered you should test and inspect your board with a multimeter according to the schematic. If you are sure about it then insert the batteries correctly and power it on.**   

![Assembling Modules](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Assembling%20Modules.jpeg)

**Note : The image above include *Rev. 1* which is the prototype version of this board. Assembly guide is identical.**

### Audio Calibration

After assembly and testing that your radio works you must calibrate the audio.

To calibrate the audio you must first lower the volume as down as you can using the volume knob of the radio. Then you must turn the variable resistor found on the audio board until you can hear the audio coming from the speaker barely. Audio is calibrated,  you should use the volume knob from now on.

## Notes

* Some power adapters are not working with this battery charger module (DDTCCRUB) because it lacks power delivery (PD) technology. If your charger doesn't work try another charger. 
* If you power the radio with DC jack while battery pack is installed, QMX+ will disconnect the batteries from radio. You can only charge the batteries from the Type-C port. QMX+'s own Type-C port is only for data.
* The 8mm x 8mm square behind the board is for JLCPCB order number. Select the **'2D Barcode' option and specify position** while ordering.

## Links

* [QRP-Labs Website](https://www.qrp-labs.com)
* [QRP-Labs QMX+ Transciever](https://qrp-labs.com/qmxp.html)

## Special thanks to G0UPL Hans Summers. This project is made possible with his help.

![Meeting](https://github.com/laxdronum/QMX-Plus-Battery-and-Audio-Board/blob/main/Images/Meeting.jpg)

# laxdronum, TA7MNA, GITRAD Radio Club YM7KK