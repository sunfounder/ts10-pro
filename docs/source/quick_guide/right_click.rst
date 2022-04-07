
Right Click on Raspberry Pi
=================================

Touchscreen tablets and displays make it easy for you to perform simple navigation tasks with your fingers or stylus, but at some point, you may want to use right-click commands to quickly access context-specific shortcuts.

Here we use ``evdev-rce`` to make right-click command still available.

Enter the following command to install the required software.

.. raw:: html

    <run></run>

.. code-block:: shell

    sudo apt install build-essential libevdev2 libevdev-dev
    git clone 'https://github.com/PeterCxy/evdev-right-click-emulation.git'
    cd 'evdev-right-click-emulation'

Enter the following command to build.

.. raw:: html

    <run></run>

.. code-block:: shell

    make all

Copy the file to the ``/usr`` directory.

.. raw:: html

    <run></run>

.. code-block:: shell

    sudo cp 'out/evdev-rce' '/usr/local/bin/'

Make it executable.

.. raw:: html

    <run></run>

.. code-block:: shell

    sudo chmod +x '/usr/local/bin/evdev-rce'

Modify the /etc/rc.local file to enable boot-up.

.. raw:: html

    <run></run>

.. code-block:: shell

    sudo nano /etc/rc.local

After entering rc.local, add the following command before ``exit 0``.

.. raw:: html

    <run></run>

.. code-block:: shell

    sudo /usr/local/bin/evdev-rce &

After restarting, you can long press on the desktop and see if the right click function appears.

.. raw:: html

    <run></run>

.. code-block:: shell

    sudo reboot

.. image:: img/right_click.png
  :align: center
