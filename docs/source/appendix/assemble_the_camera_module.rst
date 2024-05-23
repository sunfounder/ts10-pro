
.. note::

    Hello, welcome to the SunFounder Raspberry Pi & Arduino & ESP32 Enthusiasts Community on Facebook! Dive deeper into Raspberry Pi, Arduino, and ESP32 with fellow enthusiasts.

    **Why Join?**

    - **Expert Support**: Solve post-sale issues and technical challenges with help from our community and team.
    - **Learn & Share**: Exchange tips and tutorials to enhance your skills.
    - **Exclusive Previews**: Get early access to new product announcements and sneak peeks.
    - **Special Discounts**: Enjoy exclusive discounts on our newest products.
    - **Festive Promotions and Giveaways**: Take part in giveaways and holiday promotions.

    👉 Ready to explore and create with us? Click [|link_sf_facebook|] and join today!

.. _camera_module:

Assemble the Camera Module
==================================

On the camera module or Raspberry Pi, you will find a flat plastic connector. Carefully pull out the black fixing switch until the fixing switch is partially pulled out. Insert the FFC cable into the plastic connector in the direction shown and push the fixing switch back into place.

If the FFC wire is installed correctly, it will be straight and will not pull out when you gently pull on it. If not, reinstall it again.

.. image:: img/connect_ffc.png
    :align: center

.. image:: img/1.10_camera.png
    :align: center

.. warning::

    Do not install the camera with the power on, it may damage your camera.

Open **Raspberry Pi Configuration**.

.. image:: img/raspbian1.png
  :width: 550
  :align: center

In the **Interfaces** option, **Enable** the Camera, and then click **OK**.

.. image:: img/raspbian2.png
  :width: 500
  :align: center


In the pop-up prompt box, choose to restart now.

.. image:: img/raspbian3.png
  :width: 400
  :align: center

After the restart is complete, use the following command line to check whether the camera is available.

If the camera screen appears it means that the camera is installed successfully. Otherwise the FFC cable needs to be unplugged and plugged in again.

.. raw:: html

    <run></run>

.. code-block:: shell

    raspivid -o vid.h264

