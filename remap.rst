Remapping Your Keypad
=================================

.. warning::
    These remapping instructions are NOT for the Fightboard. If you have a Fightboard, the 8 right keys can be swapped by using the menu built into the controller. Please visit the Fightboard page for more information.

Every keypad has a remapper built-in to the firmware that can be accessed through a program that is able to communicate with the keypad. Please follow the instructions below for your platform.

Windows
*******

If you are on Windows 8.1 or lower and you haven't already, follow the driver installation guide first.

`Driver Installation <http://docs.thnikk.moe/en/latest/driver.html>`_

Once the drivers are installed, download and extract Termite. You want to make sure you extract since you need to run it with the .ini file in the same directory.

`Download Termite <https://puu.sh/w8Zj5/01aa028013.zip>`_

Upon opening the program, it should immediately connect to the keypad. Follow the directions in the remapper and you're all set!

* If you have any problems, make sure your settings match these (except for the port since it may be different for you):

.. image:: http://puu.sh/C8hhI/6d005fdf84.png

Make sure to close Termite when you're done, otherwise it may try to reconnect and lock up your keypad.


Universal
*********

You can also use the Serial Monitor included in the Arduino IDE. This can be done by downloading the IDE through the Arduino website here:

`Download <https://www.arduino.cc/en/Main/Software>`_

Follow the wizard for installation and launch the program. From here you can select the port from Tools > Ports and open the Serial Monitor by clicking the magnifying glass icon in the top right of the window.

.. warning::
    Make sure you change "Newline" to "No line ending" in the bottom right of the serial monitor or the keypad will think you're trying to map every key to a newline character.


Mac and Linux (Terminal)
************************************************************

The procedure for Mac and Linux is the same since we'll be using the screen command on both. This command finds the first matching serial device (should be /dev/ttyACM* on linux and /dev/cu.usbmodem* on mac) and opens a screen session with the correct baudrate.

:code:`screen $(ls -d /dev/* | grep "ACM\|usbmodem") 9600`

That's it!
