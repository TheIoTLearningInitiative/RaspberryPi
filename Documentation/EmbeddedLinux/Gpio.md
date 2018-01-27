# General Purpose Input Output (GPIO)

> General-purpose input/output (GPIO) is a generic pin on an integrated circuit whose behavior—including whether it is an input or output pin—is controllable by the user at run time. Wikipedia

- [Linux Kernel GPIO Documentation](https://www.kernel.org/doc/Documentation/gpio/)
- [LWN GPIO In The Kernel: An Introduction](https://lwn.net/Articles/532714/)
- [Wikipedia GPIO](https://en.wikipedia.org/wiki/General-purpose_input/output)

# Kernel Ring Buffer

```sh
pi@raspberrypi:~ $ dmesg | grep -i gpio
[    0.080031] uart-pl011 3f201000.serial: could not find pctldev for node /soc/gpio@7e200000/uart0_pins, deferring probe
[    3.524055] gpiomem-bcm2835 3f200000.gpiomem: Initialised: Registers at 0x3f200000
pi@raspberrypi:~ $ 
```