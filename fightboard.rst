Fightboard
===========
.. image:: https://cdn.shopify.com/s/files/1/0093/7295/8767/products/IMG_0934_1024x1024@2x.jpg?v=1583586229

Have you ever been frustrated with fightsticks? Do you want something to use on your desk that isn't a massive box you have to put away somewhere when you're not using it? Do you prefer the natural spacing of a keyboard over the finger-stretching traditional arcade buttons? Maybe you want something that you can easily use on-the-go. The Fightboard aims to solve all of those problems.

Features
********

Ergonomic layout
----------------
.. image:: https://thnikk.moe/img/fbLayout.png

The Fightboard uses a combination of an arrow/wasd cluster at a 15% angle and action buttons following the traditional arcade stick layout but with the spacing of keyboard keys.

Kailh Choc switches
-------------------
.. image:: https://thnikk.moe/img/kailhLP.jpg

Why low-profile switches? One of my main design goals for this controller was to make it as slim as possible to improve ergonomics and portability. These low-profile switches have 3mm of travel compared to the 4mm of Cherry MX switches, with an actuation point 1mm higher as well. They also help the Fightboard come in at only 22mm thick, as the lower half of the switch is also much shorter.

Hot-swap sockets
----------------
.. image:: https://thnikk.moe/img/kailhHS.png

Unhappy with your switch coice? Want different zones with different types of switches? All you have to do is pull them out and swap them with whatever you prefer, no soldering required.

RGB LEDs
--------
The RGB LEDs indicate the function of each button. The default profile uses Xbox colors for the 4 face buttons, but these can be changed to suit your preferences or the colors used in-game. The LED for each key turns off when the key is pressed and fades back on when released.

Idle mode
---------
The LEDs will turn off after a minute of inactivity. Pressing any button will turn them back on.

Easy remapping
--------------
Settings are all built into the keypad and allow you to remap keys on-the-fly.

SOCD cleaning
-------------
Left+Right will cancel each other out and Up+Down will function as Up.


Firmware
********
As of 7/6/21, a newer version of the Fightboard was released, which will be referred to in this section as the Fightboard V2. Since the V2 was released after firmware version 1.4, that is the earliest firmware version available (though I don't recommend you use earlier firmware versions anwyay.) Read the readme in the zip for installation instructions.

================ ====================================================== ========================================================
Version          Fightboard V1                                          Fightboard V2
================ ====================================================== ========================================================
1.0              `Link <https://thnikk.moe/files/FBUpdater.zip>`_       --
1.1              `Link <https://thnikk.moe/files/FBUpdater_1.1.zip>`_   --
1.2              `Link <https://thnikk.moe/files/FBUpdater_1.2.zip>`_   --
1.3              `Link <https://thnikk.moe/files/FBUpdater_1.3.zip>`_   --
1.4              `Link <https://thnikk.moe/files/FBUpdater_1.4.zip>`_   `Link <https://thnikk.moe/files/FBUpdater_RGB_1.4.zip>`_
================ ====================================================== ========================================================

There is also an alternative firmware written by Jason Skuby/FeralAI that brings native compatiblity with the Nintendo switch, but is missing features like remapping and custom LED colors. Since the V2 uses different LEDs, I've made a fork of the code specific to the V2, but any feature requests or bug reports should be made to the original author's github.

================ =================================================================================== ===========================================================
Version          Fightboard V1                                                                       Fightboard V2
================ =================================================================================== ===========================================================
0.1              `Link <https://github.com/FeralAI/FightboardHybrid/releases/tag/v0.1-alpha>`_       `Link <https://github.com/thnikk/FightboardHybrid/releases/tag/v0.1.1-alpha>`_
================ =================================================================================== ===========================================================


Compatibility
*************
The Fightboard is only compatible with PC out of the box, but can be made compatible with the adapters listed below (and the Switch with the firmware above.)

==============  ==========  =======
System          Compatible  Link
==============  ==========  =======
PC              Yes         No adapter needed
Switch          Yes         See above for alternative firmware or `Amazon (Brook) <https://www.amazon.com/Brook-Wingman-Support-Controller-Converter/dp/B08L7JQL4P>`_ /
                            `Amazon (Mayflash) <https://www.amazon.com/Mayflash-Magic-NS-Wireless-Controller-Nintendo/dp/B079B5KHWQ>`_
Xbox One        Yes         `Amazon <https://www.amazon.com/Brook-Wingman-Support-Controller-Converter/dp/B08H1SYGWV>`_
PS4             Yes         `Amazon <https://www.amazon.com/Brook-Wingman-Support-Controller-Converter/dp/B08B82M9TG>`_
Xbox 360        No          Not compatible
==============  ==========  =======


Menu
****
All settings are accessible from the controller itself by pressing left+right+home.

Direction mode
--------------
As of firmware version 1.2, you can change the directional keys to function as either a dpad or the left analog stick, since some games require one or the other. After entering the menu, you can press L3 to enable dpad mode (the keys will turn red) and R3 to enable left stick mode (the keys will turn yellow.)

Profiles
--------
From the main menu, you can press one of the 8 keys on the right to switch between 8 different profiles. These all have independent settings so you can set up each profile for a different game, each with different colors and mappings.

Button swapping
---------
You can press the start button after entering the menu to enter the button swapper. In this mode, pressing one of the 8 buttons on the right will make it pulse quickly. Press another button and the two buttons will swap places, along with their colors.

.. raw:: html

    <div>
        <video width="100%" controls>
            <source src="https://thnikk.moe/files/videos/remap.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>



Color changing
--------------
You can also press back on the main menu to enter color changing mode. Pressing one of the keys will cycle through RGB for that key.

.. raw:: html

    <div>
        <video width="100%" controls>
            <source src="https://thnikk.moe/files/videos/color.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>


.. warning::
    Remapping and color changing are only available for the 8 keys on the right. The d-pad keys are not reconfigurable.

Resetting
---------
Pressing L3 and R3 simultaneously in the main menu will clear the current profile back to its default settings.

.. raw:: html

    <div>
        <video width="100%" controls>
            <source src="https://thnikk.moe/files/videos/reset.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>



Exiting menus
-------------
Pressing the home button will always take you one step back out of a menu, meaning it will take you to the main menu on the color changer or remapper and exit from the main menu.

.. raw:: html

    <div>
        <video width="100%" controls>
            <source src="https://thnikk.moe/files/videos/menuClose.mp4" type="video/mp4">
            Your browser does not support the video tag.
        </video>
    </div>


