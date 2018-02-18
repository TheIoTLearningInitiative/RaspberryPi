# General Purpose Input Output (GPIO)

> General-purpose input/output (GPIO) is a generic pin on an integrated circuit or computer board whose behavior—including whether it is an input or output pin—is controllable by the user at run time. [Wikipedia](https://en.wikipedia.org/wiki/General-purpose_input/output)

Hardware Perspective

- [Raspberry Pi GPIO and Physical Computing](https://www.raspberrypi.org/documentation/usage/gpio-plus-and-raspi2/README.md)
- [Sparkfun Raspberry gPIo](https://learn.sparkfun.com/tutorials/raspberry-gpio/gpio-pinout)
- [Adafruit GPIO Setup](https://learn.adafruit.com/adafruits-raspberry-pi-lesson-4-gpio-setup?view=all)
- [ELinux RPi GPIO Code Samples](https://elinux.org/RPi_GPIO_Code_Samples)

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