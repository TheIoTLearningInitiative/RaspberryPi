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