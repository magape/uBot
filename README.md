# uBot

uBot is a robotic platform based on the micro:bit development board.

<img src=https://github.com/magape/uBot/blob/e107dde5819811c388ca1cb4512f05e274810612/3D/img/ubot.jpg title="uBot" width=90%>

## Mechanical assembly
The parts of uBot can be seen in the next figure.

<img src=https://github.com/magape/uBot/blob/e107dde5819811c388ca1cb4512f05e274810612/3D/img/ubot_annotated_en.png title="uBot parts" width=90%>

Some mechanical parts (chassis, motor brackets, and wheels) are 3D printed using available [stl files](https://github.com/magape/uBot/tree/main/3D/stl).
The parts are mechanically assembled with M2 nuts, bolts, and washers. The assembly can be done according to the [pictures](https://github.com/magape/uBot/tree/main/img) showing the step-by-step process.

## Electrical part

The robot is powered by a 2s LiPo battery. There are two step-down convertors which output the two necessary voltages: 3V convertor (right side) for the microcontroller and 5V convertor (left side) for motors. The two step-down convertors are assembled on two custom PCBs to be easier to mount on the robot chassis. 
The robot has a line sensor mounted on the front of the robot. The board is powered with a 3 V voltage, the same voltage as the microcontroller. Four analog signals are sent from the line sensor to the microcontroller. The line sensor contains four SMD opto-reflective sensors assembled on a custom PCB.

<img src= https://github.com/magape/uBot/blob/60dc44fdb9496fba89dab84121538997094759a6/etc/4LineSnsNoCtrl3V_sch-rgb.TIF title="Line sensor schematic" width=45%> <img src= https://github.com/magape/uBot/blob/7714591823c119a591a998ec4e5a49af790a6cc0/etc/4LineSnsNoCtrl3V_3Dbot.png title="Line sensor - bottom" width=45%>

uBot is controlled by a micro:bit board, installed on a micro:bit extension board. The microcontroller receives four analog signals from the line sensor and based on these signals computes the robot position related to the line. The microcontroller controls the speeds of the two motors, via a dual motor driver DRV8838 module, using PWM signals.

[![uBot]( https://github.com/magape/uBot/blob/14cb04c93d6d7820f3e731355ba3ac0390ead9fe/img/uBot_YouTube.png)]( https://youtu.be/6SwylmoUkn4)

## Credits

The uBot was designed by [Mihai Agape](https://github.com/magape).

## Licence

[Licensed under the Creative Commons — Attribution-ShareAlike 4.0 International — CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/)

## Note

This is a work in progress.
