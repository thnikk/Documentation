Programming Your Keypad
=======================

.. warning::
    This guide is NOT for remapping keys. Even if you do reprogram the keypad, you will only be reverting back to the default keymappings. If you'd like to remap your keys, follow the remapping guide.

PlatformIO
**********

What is it?
-----------
PlatformIO is an IDE like the Arduino IDE but is integrated with your text editor!


Download Atom
-------------
Download and install Atom from here: https://atom.io/

Install PlatformIO
------------------
Launch atom and press ctrl and comma which will open the settings menu. Click on install, type "platformio" into the search box and hit enter. Click install on "platformio-ide" and wait for it to install. It should ask if you want to install clang for auto-completion but it's not necessary so you can just ignore it. When the installation finishes, you should see a button in the top right that tells you to restart to apply the changes. Hit restart and you're good to go!

Download the Code
-----------------

Click the link for your respective model to go to the GitHub page that contains the necessary code. Click the "clone or download" button and then select "download zip." Extract it to wherever you like (I would recommend your desktop or documents folder.)

- `Basic/RGB 2K/4K <https://github.com/thnikk/trinketM0>`_
- `7K Keypad <https://github.com/thnikk/7kKeypad>`_
- `MacroPad <https://github.com/thnikk/trinketM0Macro>`_
- `Touch Keypad <https://github.com/thnikk/touchPad>`_

Uploading the code
------------------

.. image:: https://puu.sh/BgHur/d4507e79bb.png

Open the folder in Atom that you just extracted from the zip that contains the "platformio.ini" file and it should show up in the left panel under "Project." It should be called <code>-master, but make sure it's the one that contains platformio.ini since there can be two of the folders depending on how you extracted the zip. Click on the folder with the same title as the parent folder and open the file with the same title with the .ino extension (which should be something like trinketM0-master > trinketM0 > trinketM0.ino, the names will be different depending on the code you're using). Make sure your keypad is plugged in and press F7. Type "upload" and select the correct option for your model (if you don't select the model, it will try to upload all of them so make sure to do this.) You may need to try a few times and if it tells you that it can't find the port, just try unplugging the keypad and plugging it back in. If all goes well, it should upload the code to the keypad!


Making Changes to the Firmware
==============================

Understanding the basics
------------------------

There are some things you should familiarize yourself with before you get started. These are the most important functions/libararies.

`digitalRead() <https://www.arduino.cc/en/Reference/DigitalRead>`_ for reading button inputs.

`analogWrite() <https://www.arduino.cc/en/Reference/AnalogWrite>`_ for controlling single-color LEDs.

The `neopixel library <https://learn.adafruit.com/adafruit-neopixel-uberguide/arduino-library>`_ for controlling RGB LEDs.


You should also know...
-----------------------

`for loops <https://www.arduino.cc/en/Reference/For>`_

`switch/case statements <https://www.arduino.cc/en/Reference/SwitchCase>`_

`millis timers <https://learn.adafruit.com/multi-tasking-the-arduino-part-1/using-millis-for-timing>`_


I wouldn't recommend trying to change random variables unless you can actually follow the logic and see exactly what they're changing. Some of them may tie in somewhere else and cause unexpected results.
