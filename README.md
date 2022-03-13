# Firmware-Exploration-Project
The code in this repo can be used to help explore new hardware

Binary_experimentation:

// if you want copy the functions that generate the 8-bit unsigned character
// copy the code between the lines. Acces that code with in your program like this:
// unsigned char byte;
// printBinaryInput(byte);
// and your 8-bit unsigned char will be inside 'byte'


Background:
The idea for this code came up while exploring a 8X8 LED matrix module that is soldered with a MAX7219 IC. The MAX 7219 IC datasheet is written under the assumption that
the ID will be used for 7-segment displays. For that reason, it is a bit hard to understand how the module integrates it with the 8X8 LED matrix. The MAX7219 uses
serial communication so I decided to just give the module some inputs of 8-bit combinations and see what would happen. This proved to be a very annoying process.
The idea then came to have a program that continuously - in real-time - generates 8 bits as defined by the used via the command line. That way I was able to
try many different inputs to the module without reflashin code, recompiling or anything like that.

![image](https://user-images.githubusercontent.com/89616796/158040548-b1e0fd1f-9b23-4683-81c5-651df8017c62.png)
