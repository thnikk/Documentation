Troubleshooting Guide
=====================
This guide will walk you through steps to either get your keypad back up and running or properly diagnose the problem.

Connection
----------
Keypad won't turn on
***********************
This is usually caused by a problem with the USB connection. You can tell if your keypad is receiving power by looking for a faint red glow from the power LED inside.

  1) Check your cable and make sure it's plugged in all the way on both ends.
  2) Try a different cable.
  3) Check your micro-USB port to see if it's still connected to the board. In some exteme cases, it might have been ripped off.

USB device not recognized
*************************
This can be caused by a number of things, the most common two being a bad USB connection or a corrupted/incorrect bootloader.

  1) Follow the steps for the previous issue
  2) If you've recently tried uploading new code, open the keypad and quickly short the GND and RST pins twice. This will force it back into bootloader mode and you should be able to reupload your code. Make sure you have the correct board selected.

Shows up in Device Manager but it still isn't working
*****************************************************

  1) Make sure you don't have a serial monitor open anywhere that may be falsely triggering the keypad to enter remap mode.
  2) Try following the reprogramming guide to get the stock code back on the keypad.


The remapper isn't working with Termite
***************************************
This is most commonly caused by having the Arduino Create plugin running. You can either disable it through the system tray in the bottom right or you can just use the Arduino Create serial monitor.


Mechanical
----------
One of my switches isn't working consistently
*********************************************
Try removing the o-rings from the keycaps to see if they are preventing the keys from being fully depressed.


Programming
-----------
It's not compiling and giving me an error
*****************************************

  1) Enable verbose output for compilation and uploading under File>Preferences.
  2) Make sure you installed the required libraries (bounce2 and neopixel) under Sketch>Include Library>Manage Libraries...

It won't upload
***************
Make sure that you have the correct board and port selected.You need to select Arduino Leonardo under Tools>Boards and the port should be labeled with (Arduino Leonardo) next to it under Tools>Ports.

Remapping (on Remapper 1.1)
---------------------------
The keys I enter aren't mapping properly
****************************************
1) Make sure you're entering your modifiers first.
2) Make sure you're only entering three keys (including modifiers.)
3) Enter xx (lowercase) after entering a modifier if you don't wish for any additional keys to be mapped to that key. Otherwise, enter the remaining keys.
