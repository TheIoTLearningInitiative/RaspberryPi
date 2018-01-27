# Modules

> In computing, a loadable kernel module (or LKM) is an object file that contains code to extend the running kernel, or so-called base kernel, of an operating system. LKMs are typically used to add support for new hardware (as device drivers) and/or filesystems, or for adding system calls. [Wikipedia](https://en.wikipedia.org/wiki/Loadable_kernel_module)

## Command lsmod

```sh
pi@raspberrypi:~ $ lsmod
Module                  Size  Used by
fuse                   99603  3
cmac                    3239  1
rfcomm                 37723  6
bnep                   12051  2
hci_uart               20020  1
btbcm                   7916  1 hci_uart
bluetooth             365780  29 hci_uart,bnep,btbcm,rfcomm
brcmfmac              292632  0
brcmutil                9863  1 brcmfmac
cfg80211              544545  1 brcmfmac
rfkill                 20851  6 bluetooth,cfg80211
snd_bcm2835            24427  1
snd_pcm                98501  1 snd_bcm2835
snd_timer              23968  1 snd_pcm
snd                    70032  5 snd_timer,snd_bcm2835,snd_pcm
bcm2835_gpiomem         3940  0
joydev                  9988  0
evdev                  12423  3
uio_pdrv_genirq         3923  0
fixed                   3285  0
uio                    10204  1 uio_pdrv_genirq
i2c_dev                 6913  0
ip_tables              13161  0
x_tables               20578  1 ip_tables
ipv6                  408900  40
pi@raspberrypi:~ $ 
```

## Command modinfo

```sh
pi@raspberrypi:~ $ modinfo snd_bcm2835
filename:       /lib/modules/4.9.59-v7+/kernel/sound/arm/snd-bcm2835.ko
alias:          platform:bcm2835_alsa
license:        GPL
description:    Alsa driver for BCM2835 chip
author:         Dom Cobley
srcversion:     B872A627E265EFD08A9A41B
alias:          of:N*T*Cbrcm,bcm2835-audioC*
alias:          of:N*T*Cbrcm,bcm2835-audio
depends:        snd-pcm,snd
intree:         Y
vermagic:       4.9.59-v7+ SMP mod_unload modversions ARMv7 p2v8 
parm:           force_bulk:Force use of vchiq bulk for audio (bool)
pi@raspberrypi:~ $ 
```

```sh
for mod in `cat /proc/modules | cut -d " " -f 1`
do
    desc=`modinfo -d $mod`
    printf "%-20s $desc\n" "$mod:"
done
```

```sh
fuse:                Filesystem in Userspace
cmac:                CMAC keyed hash algorithm
rfcomm:              Bluetooth RFCOMM ver 1.11
bnep:                Bluetooth BNEP ver 1.3
hci_uart:            Bluetooth HCI UART driver ver 2.3
btbcm:               Bluetooth support for Broadcom devices ver 0.1
bluetooth:           Bluetooth Core ver 2.22
brcmfmac:            Broadcom 802.11 wireless LAN fullmac driver.
brcmutil:            Broadcom 802.11n wireless LAN driver utilities.
cfg80211:            wireless configuration support
rfkill:              RF switch support
snd_bcm2835:         Alsa driver for BCM2835 chip
snd_pcm:             Midlevel PCM code for ALSA.
snd_timer:           ALSA timer interface
snd:                 Advanced Linux Sound Architecture driver for soundcards.
bcm2835_gpiomem:     gpiomem driver for accessing GPIO from userspace
joydev:              Joystick device interfaces
evdev:               Input driver event char devices
uio_pdrv_genirq:     Userspace I/O platform driver with generic IRQ handling
fixed:               Fixed voltage regulator
uio:                 
i2c_dev:             I2C /dev entries driver
ip_tables:           IPv4 packet filter
x_tables:            {ip,ip6,arp,eb}_tables backend module
ipv6:                IPv6 protocol stack for Linux
```

