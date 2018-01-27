# Processes

## Command ps

```sh
PS(1)                            User Commands                           PS(1)

NAME
       ps - report a snapshot of the current processes.

SYNOPSIS
       ps [options]

DESCRIPTION
       ps displays information about a selection of the active processes.  If
       you want a repetitive update of the selection and the displayed
       information, use top(1) instead.
...
```

```sh
pi@raspberrypi:~ $ ps -aux
USER       PID %CPU %MEM    VSZ   RSS TTY      STAT START   TIME COMMAND
root         1  0.0  0.6  26932  5964 ?        Ss   03:53   0:01 /sbin/init splash
root         2  0.0  0.0      0     0 ?        S    03:53   0:00 [kthreadd]
root         3  0.0  0.0      0     0 ?        S    03:53   0:00 [ksoftirqd/0]
root         5  0.0  0.0      0     0 ?        S<   03:53   0:00 [kworker/0:0H]
root         7  0.0  0.0      0     0 ?        S    03:53   0:02 [rcu_sched]
root         8  0.0  0.0      0     0 ?        S    03:53   0:00 [rcu_bh]
root         9  0.0  0.0      0     0 ?        S    03:53   0:00 [migration/0]
root        10  0.0  0.0      0     0 ?        S<   03:53   0:00 [lru-add-drain]
root        11  0.0  0.0      0     0 ?        S    03:53   0:00 [cpuhp/0]
root        12  0.0  0.0      0     0 ?        S    03:53   0:00 [cpuhp/1]
root        13  0.0  0.0      0     0 ?        S    03:53   0:00 [migration/1]
root        14  0.0  0.0      0     0 ?        S    03:53   0:00 [ksoftirqd/1]
root        16  0.0  0.0      0     0 ?        S<   03:53   0:00 [kworker/1:0H]
root        17  0.0  0.0      0     0 ?        S    03:53   0:00 [cpuhp/2]
root        18  0.0  0.0      0     0 ?        S    03:53   0:00 [migration/2]
root        19  0.0  0.0      0     0 ?        S    03:53   0:00 [ksoftirqd/2]
root        21  0.0  0.0      0     0 ?        S<   03:53   0:00 [kworker/2:0H]
root        22  0.0  0.0      0     0 ?        S    03:53   0:00 [cpuhp/3]
root        23  0.0  0.0      0     0 ?        S    03:53   0:00 [migration/3]
root        24  0.0  0.0      0     0 ?        S    03:53   0:00 [ksoftirqd/3]
root        26  0.0  0.0      0     0 ?        S<   03:53   0:00 [kworker/3:0H]
root        27  0.0  0.0      0     0 ?        S    03:53   0:00 [kdevtmpfs]
root        28  0.0  0.0      0     0 ?        S<   03:53   0:00 [netns]
root        29  0.0  0.0      0     0 ?        S    03:53   0:00 [khungtaskd]
root        30  0.0  0.0      0     0 ?        S    03:53   0:00 [oom_reaper]
root        31  0.0  0.0      0     0 ?        S<   03:53   0:00 [writeback]
root        32  0.0  0.0      0     0 ?        S    03:53   0:00 [kcompactd0]
root        33  0.0  0.0      0     0 ?        S<   03:53   0:00 [crypto]
root        34  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        35  0.0  0.0      0     0 ?        S<   03:53   0:00 [kblockd]
root        36  0.0  0.0      0     0 ?        S<   03:53   0:00 [watchdogd]
root        38  0.0  0.0      0     0 ?        S<   03:53   0:00 [rpciod]
root        39  0.0  0.0      0     0 ?        S<   03:53   0:00 [xprtiod]
root        40  0.0  0.0      0     0 ?        S    03:53   0:00 [kswapd0]
root        41  0.0  0.0      0     0 ?        S<   03:53   0:00 [vmstat]
root        42  0.0  0.0      0     0 ?        S<   03:53   0:00 [nfsiod]
root        52  0.0  0.0      0     0 ?        S<   03:53   0:00 [kthrotld]
root        53  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        54  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        55  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        56  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        57  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        58  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        59  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        60  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        61  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        62  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        63  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        64  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        65  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        66  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        67  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        68  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        69  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        70  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        71  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        72  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        73  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        74  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        75  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        76  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        77  0.0  0.0      0     0 ?        S<   03:53   0:00 [iscsi_eh]
root        78  0.0  0.0      0     0 ?        S<   03:53   0:00 [dwc_otg]
root        79  0.0  0.0      0     0 ?        S    03:53   0:00 [kworker/2:1]
root        80  0.0  0.0      0     0 ?        S<   03:53   0:00 [DWC Notificatio]
root        81  0.0  0.0      0     0 ?        S<   03:53   0:00 [VCHIQ-0]
root        82  0.0  0.0      0     0 ?        S<   03:53   0:00 [VCHIQr-0]
root        83  0.0  0.0      0     0 ?        S<   03:53   0:00 [VCHIQs-0]
root        84  0.0  0.0      0     0 ?        S    03:53   0:00 [VCHIQka-0]
root        85  0.0  0.0      0     0 ?        S<   03:53   0:00 [SMIO]
root        87  0.0  0.0      0     0 ?        S    03:53   0:00 [irq/92-mmc1]
root        90  0.0  0.0      0     0 ?        S<   03:53   0:00 [bioset]
root        91  0.0  0.0      0     0 ?        S    03:53   0:01 [mmcqd/0]
root        93  0.0  0.0      0     0 ?        S    03:53   0:00 [jbd2/mmcblk0p2-]
root        94  0.0  0.0      0     0 ?        S<   03:53   0:00 [ext4-rsv-conver]
root        95  0.0  0.0      0     0 ?        S<   03:53   0:00 [ipv6_addrconf]
root       118  0.0  0.4  35112  4572 ?        Ss   03:53   0:00 /lib/systemd/systemd-journald
root       151  0.0  0.3  14680  3432 ?        Ss   03:53   0:00 /lib/systemd/systemd-udevd
root       243  0.0  0.0      0     0 ?        S<   03:53   0:00 [cfg80211]
root       252  0.0  0.0      0     0 ?        S<   03:53   0:00 [brcmf_wq/mmc1:0]
root       253  0.0  0.0      0     0 ?        S    03:53   0:00 [brcmf_wdog/mmc1]
systemd+   297  0.0  0.4  17280  3928 ?        Ssl  03:53   0:00 /lib/systemd/systemd-timesyncd
avahi      324  0.0  0.3   6400  3100 ?        Ss   03:53   0:01 avahi-daemon: running [raspberrypi.local]
root       326  0.0  0.4   7376  4280 ?        Ss   03:53   0:00 /lib/systemd/systemd-logind
root       330  0.0  0.2   5292  2376 ?        Ss   03:53   0:00 /usr/sbin/cron -f
message+   332  0.0  0.3   6604  3596 ?        Ss   03:53   0:00 /usr/bin/dbus-daemon --system --address=systemd: --nofork --nopidfile --systemd-activation
avahi      350  0.0  0.0   6400   328 ?        S    03:53   0:00 avahi-daemon: chroot helper
root       351  0.0  0.1   2948  1820 ?        Ss   03:53   0:00 /sbin/dhcpcd -q -b
root       369  0.0  0.2  23748  2728 ?        Ssl  03:53   0:00 /usr/sbin/rsyslogd -n
nobody     372  0.0  0.2   5292  2492 ?        Ss   03:53   0:00 /usr/sbin/thd --triggers /etc/triggerhappy/triggers.d/ --socket /run/thd.socket --user nobody --deviceg
root       393  0.0  0.3  10128  3000 ?        Ss   03:53   0:00 wpa_supplicant -B -c/etc/wpa_supplicant/wpa_supplicant.conf -iwlan0 -Dnl80211,wext
root       453  0.0  0.7  39964  7328 ?        Ssl  03:53   0:00 /usr/sbin/lightdm
root       454  0.0  0.0      0     0 ?        S<   03:53   0:00 [kworker/2:1H]
root       457  0.0  0.3   5880  2940 tty1     Ss   03:53   0:00 /bin/login -f
root       463  4.1  6.1 180784 58432 tty7     Ssl+ 03:53   2:07 /usr/lib/xorg/Xorg :0 -seat seat0 -auth /var/run/lightdm/root/:0 -nolisten tcp vt7 -novtswitch
root       476  0.0  0.0      0     0 ?        S<   03:54   0:00 [kworker/u9:0]
root       477  0.0  0.0      0     0 ?        S<   03:54   0:00 [hci0]
root       478  0.0  0.0      0     0 ?        S<   03:54   0:00 [hci0]
root       479  0.0  0.0   2096   152 ?        S    03:54   0:00 /usr/bin/hciattach /dev/serial1 bcm43xx 921600 noflow - b8:27:eb:c2:70:5e
root       480  0.0  0.0      0     0 ?        S<   03:54   0:00 [kworker/u9:1]
root       485  0.0  0.3   7268  3668 ?        Ss   03:54   0:00 /usr/lib/bluetooth/bluetoothd
root       487  0.0  0.3  35036  3504 ?        Ssl  03:54   0:00 /usr/bin/bluealsa
root       502  0.0  0.0      0     0 ?        S<   03:54   0:00 [krfcommd]
pi         511  0.0  0.6   9660  5840 ?        Ss   03:54   0:00 /lib/systemd/systemd --user
pi         515  0.0  0.1  11188  1284 ?        S    03:54   0:00 (sd-pam)
pi         526  0.0  0.4   6176  4052 tty1     S+   03:54   0:00 -bash
root       547  0.0  0.7  32184  7568 ?        Sl   03:54   0:00 lightdm --session-child 14 17
pi         556  0.0  1.3  52632 12924 ?        Ssl  03:54   0:01 /usr/bin/lxsession -s LXDE-pi -e LXDE
pi         565  0.0  0.3   6508  3484 ?        Ss   03:54   0:00 /usr/bin/dbus-daemon --session --address=systemd: --nofork --nopidfile --systemd-activation
pi         604  0.0  0.1   3792  1064 ?        Ss   03:54   0:00 /usr/bin/ssh-agent x-session-manager
pi         610  0.0  0.6  39648  5888 ?        Ssl  03:54   0:00 /usr/lib/gvfs/gvfsd
pi         615  0.0  0.6  56484  6520 ?        Sl   03:54   0:00 /usr/lib/gvfs/gvfsd-fuse /run/user/1000/gvfs -f -o big_writes
pi         631  0.1  1.5  54168 14900 ?        S    03:54   0:05 openbox --config-file /home/pi/.config/openbox/lxde-pi-rc.xml
pi         634  0.0  0.9  43096  8924 ?        Sl   03:54   0:00 lxpolkit
pi         636  0.5  2.7 149188 26080 ?        Sl   03:54   0:15 lxpanel --profile LXDE-pi
pi         638  0.0  2.5 101340 24384 ?        Sl   03:54   0:01 pcmanfm --desktop --profile LXDE-pi
pi         644  0.0  0.0   3792   232 ?        Ss   03:54   0:00 /usr/bin/ssh-agent -s
root       654  0.0  0.7  40180  7296 ?        Ssl  03:54   0:00 /usr/lib/policykit-1/polkitd --no-debug
pi         674  0.0  0.6  28444  6328 ?        Ssl  03:54   0:00 /usr/lib/menu-cache/menu-cached /run/user/1000/menu-cached-:0
pi         688  0.0  1.1  74524 10648 ?        Ssl  03:54   0:00 /usr/lib/gvfs/gvfs-udisks2-volume-monitor
root       691  0.0  0.9  59240  8884 ?        Ssl  03:54   0:00 /usr/lib/udisks2/udisksd --no-debug
pi         699  0.0  0.5  38836  5128 ?        Ssl  03:54   0:00 /usr/lib/gvfs/gvfs-gphoto2-volume-monitor
pi         703  0.0  0.4  37264  4680 ?        Ssl  03:54   0:00 /usr/lib/gvfs/gvfs-mtp-volume-monitor
pi         708  0.0  0.5  50964  4872 ?        Ssl  03:54   0:00 /usr/lib/gvfs/gvfs-afc-volume-monitor
pi         717  0.0  0.5  37340  5288 ?        Ssl  03:54   0:00 /usr/lib/gvfs/gvfs-goa-volume-monitor
pi         753  0.0  0.8  51336  7916 ?        Sl   03:54   0:00 /usr/lib/gvfs/gvfsd-trash --spawner :1.4 /org/gtk/gvfs/exec_spaw/0
pi         759  0.8  2.3  51088 22152 ?        Rl   03:54   0:26 lxterminal
pi         760  0.0  0.1   2360  1392 ?        S    03:54   0:00 gnome-pty-helper
pi         761  0.0  0.4   6108  4060 pts/0    Ss   03:54   0:00 bash
root       847  0.0  0.0      0     0 ?        S<   03:54   0:00 [kworker/1:1H]
root       848  0.0  0.0      0     0 ?        S<   03:54   0:00 [kworker/0:1H]
root       849  0.0  0.0      0     0 ?        S<   03:54   0:00 [kworker/3:1H]
pi        1011 15.0 20.3 677200 193444 ?       Sl   03:55   7:22 /usr/lib/chromium-browser/chromium-browser --disable-quic --enable-fast-unload --enable-tcp-fast-open -
pi        1030  0.0  3.3 201536 31972 ?        S    03:56   0:00 /usr/lib/chromium-browser/chromium-browser --type=zygote --ppapi-flash-path=/usr/lib/chromium-browser/l
pi        1032  0.0  0.7 201536  7364 ?        S    03:56   0:00 /usr/lib/chromium-browser/chromium-browser --type=zygote --ppapi-flash-path=/usr/lib/chromium-browser/l
pi        1208  1.4 12.3 450624 117352 ?       Sl   03:56   0:43 /usr/lib/chromium-browser/chromium-browser --type=renderer --disable-gpu-compositing --enable-pinch --f
pi        1221  0.0  5.8 277672 55992 ?        Sl   03:56   0:00 /usr/lib/chromium-browser/chromium-browser --type=gpu-process --field-trial-handle=15366985519213327610
pi        1357 40.0 20.2 481204 191900 ?       Sl   03:57  19:00 /usr/lib/chromium-browser/chromium-browser --type=renderer --disable-gpu-compositing --enable-pinch --f
pi        1412  5.3 15.5 443080 147304 ?       Sl   03:59   2:24 /usr/lib/chromium-browser/chromium-browser --type=renderer --disable-gpu-compositing --enable-pinch --f
root      1451  0.0  0.0      0     0 ?        S    04:02   0:00 [kworker/1:0]
pi        1601  0.2 10.8 389320 103124 ?       Sl   04:10   0:05 /usr/lib/chromium-browser/chromium-browser --type=renderer --disable-gpu-compositing --enable-pinch --f
root      1644  0.0  0.0      0     0 ?        S    04:14   0:00 [kworker/u8:0]
root      1651  0.0  0.0      0     0 ?        S    04:15   0:00 [kworker/3:1]
root      1655  0.0  0.0      0     0 ?        S    04:16   0:00 [kworker/2:0]
root      1730  0.0  0.0      0     0 ?        S    04:20   0:00 [kworker/1:2]
root      1954  0.0  0.0      0     0 ?        S    04:31   0:00 [kworker/0:0]
root      2021  0.0  0.0      0     0 ?        S    04:33   0:00 [kworker/u8:1]
root      2030  0.0  0.0      0     0 ?        S    04:35   0:00 [kworker/3:0]
root      2090  0.0  0.0      0     0 ?        S    04:37   0:00 [kworker/0:1]
root      2091  0.0  0.0      0     0 ?        S    04:37   0:00 [kworker/2:2]
root      2181  0.0  0.0      0     0 ?        S    04:41   0:00 [kworker/u8:2]
root      2182  0.0  0.0      0     0 ?        S    04:41   0:00 [kworker/3:2]
root      2222  0.0  0.0      0     0 ?        S    04:43   0:00 [kworker/0:2]
root      2267  0.0  0.0      0     0 ?        S    04:43   0:00 [kworker/2:3]
pi        2273  0.0  0.3   7736  2884 pts/0    R+   04:44   0:00 ps -aux
pi@raspberrypi:~ $ 
```