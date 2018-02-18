# General Purpose Input Output (GPIO)

> General-purpose input/output (GPIO) is a generic pin on an integrated circuit or computer board whose behavior—including whether it is an input or output pin—is controllable by the user at run time. [Wikipedia](https://en.wikipedia.org/wiki/General-purpose_input/output)

Hardware Perspective

> _One powerful feature of the Raspberry Pi is the row of GPIO (general purpose input/output) pins along the top edge of the board._ [Homepage](https://www.raspberrypi.org/documentation/usage/gpio-plus-and-raspi2/README.md)

> _The comprehensive GPIO Pinout guide for the Raspberry Pi._ [Pinout Homepage](https://pinout.xyz/#)

> _The Raspberry Pi offers up its GPIO over a standard male header on the board. Over the years the header has expanded from 26 pins to 40 pins while maintaining the original pinout._ [Sparkfun Raspberry gPIo](https://learn.sparkfun.com/tutorials/raspberry-gpio/gpio-pinout)

> One of the great things about the Raspberry Pi is that it has a GPIO connector to which you can attach external hardware. [Adafruit GPIO Setup](https://learn.adafruit.com/adafruits-raspberry-pi-lesson-4-gpio-setup?view=all)

> _The Raspberry Pi GPIOs can be controlled using many programming languages._ [ELinux RPi GPIO Code Samples](https://elinux.org/RPi_GPIO_Code_Samples)

Operating System Perspective

- [Linux Kernel GPIO Documentation](https://www.kernel.org/doc/Documentation/gpio/)
- [LWN GPIO In The Kernel: An Introduction](https://lwn.net/Articles/532714/)
- [Wikipedia GPIO](https://en.wikipedia.org/wiki/General-purpose_input/output)

## Kernel Ring Buffer

```sh
pi@raspberrypi:~ $ dmesg | grep -i gpio
[    0.080031] uart-pl011 3f201000.serial: could not find pctldev for node /soc/gpio@7e200000/uart0_pins, deferring probe
[    3.524055] gpiomem-bcm2835 3f200000.gpiomem: Initialised: Registers at 0x3f200000
pi@raspberrypi:~ $ 
```

## SysFs

> GPIO Sysfs Interface for Userspace. Platforms which use the "gpiolib" implementors framework may choose to configure a sysfs user interface to GPIOs. This is different from the debugfs interface, since it provides control over GPIO direction and value instead of just showing a gpio state summary. Plus, it could be present on production systems without debugging support. []()

```sh
pi@raspberrypi:~ $ cd /sys/class/gpio/
pi@raspberrypi:/sys/class/gpio $ tree -L 1
.
├── export
├── gpiochip0 -> ../../devices/platform/soc/3f200000.gpio/gpio/gpiochip0
├── gpiochip100 -> ../../devices/gpiochip2/gpio/gpiochip100
├── gpiochip128 -> ../../devices/gpiochip1/gpio/gpiochip128
└── unexport

3 directories, 2 files
pi@raspberrypi:/sys/class/gpio $ 
```