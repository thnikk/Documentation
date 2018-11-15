Remapping Your Keypad
=================================

Windows
*******

If you are on Windows 8.1 or lower and you haven't already, follow the driver installation guide first.

`Driver Installation <http://docs.thnikk.moe/en/latest/driver.html>`_

Once the drivers are installed, download and extract Termite. You want to make sure you extract since you need to run it with the .ini file in the same directory.

`Download Termite <https://puu.sh/w8Zj5/01aa028013.zip>`_

* Package updated 1/19/17

  * Changed font to monospaced
  * Enabled setting to keep connection active when window isn't focused
  * Enabled word wrap

Upon opening the program, it should immediately connect to the keypad. Follow the directions in the remapper and you're all set!

Make sure to close Termite when you're done, otherwise it may try to reconnect and lock up your keypad.

.. image:: https://puu.sh/BRO0B/d9a97fe6dd.zip

Mac and Linux
*************

The procedure for Mac and Linux is the same since we'll be using the screen command on both. As we do on windows, you'll first need to find the com port the keypad is using. You can do so by entering this into the terminal:

:code:`dmesg | grep tty`

If you just plugged the keypad in, it should be the last thing listed. In my case it's using /dev/ttyACM0. Now we can start serial communications using screen.

:code:`screen /dev/ttyACM0 9600`

That's it!


Universal
*********

You can also use the Serial Monitor included in the Arduino IDE. This can be done by downloading the IDE through the Arduino website here:

`Download <https://www.arduino.cc/en/Main/Software>`_

Follow the wizard for installation and launch the program. From here you can select the port from Tools > Ports and open the Serial Monitor by clicking the magnifying glass icon in the top right of the window.
