uDraw PS3 MacOS Driver (WIP)
======================

Quick&dirty driver for the PS3 uDraw graphics tablet. If customization
is needed, hack the source.

For a Windows driver, see: http://brandonw.net/udraw/

For a Linux driver (that this was based on), see: https://github.com/TheSandBoxMKG/udraw-driver


Requirements:
-------------
* git
* homebrew
* cmake (brew)
* pkg-config (brew)
* libusb (brew)
* boost (brew) (currently isn't loading in properly)
* g++


Compilation:
------------

    mkdir build
    cd build
    cmake ..
    make


Running:
--------

Plug in the USB dongle for the graphics tablet, switch on the graphics
tablet and sync up as usual, then run one of the following commands
depending on your needs:

    udraw-driver --touchpad

    udraw-driver --tablet

    udraw-driver --gamepad

    udraw-driver --keyboard

    udraw-driver --accelerometer
