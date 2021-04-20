# SplitKeeb

### SplitKeeb is my custom designed split keyboard based on the QMK Firmware and 2 Arduino Pro Micros.

![Split Keyboard](https://i.imgur.com/FZMVq06.jpg)
(No keycaps because I can't afford them at the moment :])

![KiCad view](https://i.imgur.com/sWV3AiR.png)

![Real Life PCB](https://i.imgur.com/Sz99NFG.jpg)

This is a *split* keyboard design, and uses I2C to communicate over a TRRS audio cable (4 poles). 

The parts list is as follows:
* 62 of any Cherry MX style key Switch
* 62 1N4148 Zener Diodes
* 2 identical Resistors from a range of 2.2k Ohms to 10k Ohms (4.7k recommended) 
* 2 Arduino Pro Micros
* 2 PJ-320A TRRS Female Jacks
* 1 TRRS Male to Male wire
* 10 M3 x 8mm Bolts
* 10 M3 nuts

The 2 resistors are for the I2C line, make sure to solder them to whichever board you want to use as the 'main' side.

Make sure to plug in the TRRS cable **BEFORE** you plug in the USB cable, otherwise you risk shorts as the TRRS cable supplies power to the other board.

To program the keyboard, the eaisest method is to use the (QMK Toolbox)[https://github.com/qmk/qmk_toolbox], and flash both Pro Micros with the same 'SplitKeeb.hex' file. After both boards have been flashed, plug in the TRRS cable, and then plug in USB, and the keyboard should work as normal. 

Thanks to Rayyan and David for helping me figure out the firmware :)

