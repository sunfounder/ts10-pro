FAQ
=============

Issue 1: Black border appears on the display?
--------------------------------------------------

    * Select the correct resolution
    
    Click the **Raspberry Pi icon** -> **Preferences** -> **Screen Configuration**.

    .. image:: img/screen_config.png

    Then choose **Configure** -> **Screens** -> **HDMI-1** -> **Resolution** -> choose the 1280x800.

    .. image:: img/resolution.png

    After that you need to click the tick icon to save your configure.

    .. image:: img/hdmi1.png

    * Disable Overscan/Underscan

    When using Raspberry Pi Imager to install a system on a Micro SD, you can check the Disable overscan.

    .. image:: img/oversccan.png

    Or when you get to the desktop, click the **Raspberry Pi icon** -> **Preferences** -> **Raspberry Pi Configuration**.
    
    .. image:: img/screen_config.png

    Disable Overscan in the Display page.

    .. image:: img/disable_overscan.png

Issue 2: No Sound
----------------------

    * If your display has no sound, you need to confirm the current Audio output mode. Analog mode is used to output to the headphones, and HDMI mode is output to the speakers.
    
    .. image:: img/hdmi_analog.png

    * Make sure that the speaker wires are well connected.
    * Adjust the volume level by using the buttons on the driver board. If there is still no sound, please contact us.

The screen shows No Signal after the device is turned on?
-------------------------------------------------------------

    * Please check if all the cables are plugged in properly.
    * Check if the control board (Raspberry Pi) is on.
    * Check if the SD card has the correct system installed.

Can't touch?
-------------

    * Make sure the touch module is connected to the control board (or device) via the USB touch cable.
    * Check if the touch module is damaged, if so please contact us.

Use of the touch pen
-------------------------

    * This display works with passive capacitive stylus, while active capacitive does not.

The LCD display cannot be turned on without connecting other devices.
-----------------------------------------------------------------------

    * This is a normal phenomenon, please use it after connecting Raspberry Pi or other devices.