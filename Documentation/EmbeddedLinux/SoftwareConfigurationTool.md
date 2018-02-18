# Software Configuration Tool

> __raspi-config__ is the Raspberry Pi configuration tool [Homepage](https://www.raspberrypi.org/documentation/configuration/raspi-config.md)

```sh
pi@raspberrypi:~ $ sudo raspi-config 

Raspberry Pi Software Configuration Tool (raspi-config) 
1 Change User Password Change password for the current user
2 Network Options      Configure network settings
3 Boot Options         Configure options for start-up
4 Localisation Options Set up language and regional settings to match your location
5 Interfacing Options  Configure connections to peripherals
6 Overclock            Configure overclocking for your Pi
7 Advanced Options     Configure advanced settings
8 Update               Update this tool to the latest version
9 About raspi-config   Information about this configuration tool                              ```

> __Interfacing Options__ _Configure connections to peripherals_

```sh
P1 Camera      Enable/Disable connection to the Raspberry Pi Camera
P2 SSH         Enable/Disable remote command line access to your Pi using SSH
P3 VNC         Enable/Disable graphical remote access to your Pi using RealVNC
P4 SPI         Enable/Disable automatic loading of SPI kernel module
P5 I2C         Enable/Disable automatic loading of I2C kernel module
P6 Serial      Enable/Disable shell and kernel messages on the serial connection
P7 1-Wire      Enable/Disable one-wire interface
P8 Remote GPIO Enable/Disable remote access to GPIO pins
```

> __Advanced Options__ _Configure advanced settings_

```sh
A1 Expand Filesystem Ensures that all of the SD card storage is available to the OS
A2 Overscan          You may need to configure overscan if black bars are present on display
A3 Memory Split      Change the amount of memory made available to the GPU
A4 Audio             Force audio out through HDMI or 3.5mm jack
A5 Resolution        Set a specific screen resolution
A6 Pixel Doubling    Enable/Disable 2x2 pixel mapping
A7 GL Driver         Enable/Disable experimental desktop GL driver
```