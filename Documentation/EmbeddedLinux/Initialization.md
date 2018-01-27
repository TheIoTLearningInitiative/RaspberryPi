# Initialization

* [Gitbook Linux Initialization by 0xAX](https://0xax.gitbooks.io/linux-insides/content/)

```sh
[    0.000000] Booting Linux on physical CPU 0x0
[    0.000000] Linux version 4.9.59-v7+ (dc4@dc4-XPS13-9333) (gcc version 4.9.3 (crosstool-NG crosstool-ng-1.22.0-88-g8460611) ) #1047 SMP Sun Oct 29 12:19:23 GMT 2017
[    0.000000] CPU: ARMv7 Processor [410fd034] revision 4 (ARMv7), cr=10c5383d
[    0.000000] CPU: div instructions available: patching division code
[    0.000000] CPU: PIPT / VIPT nonaliasing data cache, VIPT aliasing instruction cache
[    0.000000] OF: fdt:Machine model: Raspberry Pi 3 Model B Rev 1.2
[    0.000000] cma: Reserved 8 MiB at 0x3ac00000
[    0.000000] Memory policy: Data cache writealloc
[    0.000000] On node 0 totalpages: 242688
[    0.000000] free_area_init_node: node 0, pgdat 80c6f380, node_mem_map ba3a1000
[    0.000000]   Normal zone: 2133 pages used for memmap
[    0.000000]   Normal zone: 0 pages reserved
[    0.000000]   Normal zone: 242688 pages, LIFO batch:31
[    0.000000] percpu: Embedded 14 pages/cpu @ba35b000 s25600 r8192 d23552 u57344
[    0.000000] pcpu-alloc: s25600 r8192 d23552 u57344 alloc=14*4096
[    0.000000] pcpu-alloc: [0] 0 [0] 1 [0] 2 [0] 3 
[    0.000000] Built 1 zonelists in Zone order, mobility grouping on.  Total pages: 240555
[    0.000000] Kernel command line: 8250.nr_uarts=0 bcm2708_fb.fbwidth=1360 bcm2708_fb.fbheight=768 bcm2708_fb.fbswap=1 vc_mem.mem_base=0x3ec00000 vc_mem.mem_size=0x40000000  dwc_otg.lpm_enable=0 console=ttyS0,115200 console=tty1 root=PARTUUID=00aa1cb9-02 rootfstype=ext4 elevator=deadline fsck.repair=yes rootwait quiet splash plymouth.ignore-serial-consoles
[    0.000000] PID hash table entries: 4096 (order: 2, 16384 bytes)
[    0.000000] Dentry cache hash table entries: 131072 (order: 7, 524288 bytes)
[    0.000000] Inode-cache hash table entries: 65536 (order: 6, 262144 bytes)
[    0.000000] Memory: 940364K/970752K available (7168K kernel code, 486K rwdata, 2012K rodata, 1024K init, 770K bss, 22196K reserved, 8192K cma-reserved)
[    0.000000] Virtual kernel memory layout:
                   vector  : 0xffff0000 - 0xffff1000   (   4 kB)
                   fixmap  : 0xffc00000 - 0xfff00000   (3072 kB)
                   vmalloc : 0xbb800000 - 0xff800000   (1088 MB)
                   lowmem  : 0x80000000 - 0xbb400000   ( 948 MB)
                   modules : 0x7f000000 - 0x80000000   (  16 MB)
                     .text : 0x80008000 - 0x80800000   (8160 kB)
                     .init : 0x80b00000 - 0x80c00000   (1024 kB)
                     .data : 0x80c00000 - 0x80c79834   ( 487 kB)
                      .bss : 0x80c7b000 - 0x80d3b964   ( 771 kB)
[    0.000000] SLUB: HWalign=64, Order=0-3, MinObjects=0, CPUs=4, Nodes=1
[    0.000000] Hierarchical RCU implementation.
[    0.000000] 	Build-time adjustment of leaf fanout to 32.
[    0.000000] NR_IRQS:16 nr_irqs:16 16
[    0.000000] arm_arch_timer: Architected cp15 timer(s) running at 19.20MHz (phys).
[    0.000000] clocksource: arch_sys_counter: mask: 0xffffffffffffff max_cycles: 0x46d987e47, max_idle_ns: 440795202767 ns
[    0.000007] sched_clock: 56 bits at 19MHz, resolution 52ns, wraps every 4398046511078ns
[    0.000019] Switching to timer-based delay loop, resolution 52ns
[    0.000295] Console: colour dummy device 80x30
[    0.000310] console [tty1] enabled
[    0.000330] Calibrating delay loop (skipped), value calculated using timer frequency.. 38.40 BogoMIPS (lpj=192000)
[    0.000345] pid_max: default: 32768 minimum: 301
[    0.000651] Mount-cache hash table entries: 2048 (order: 1, 8192 bytes)
[    0.000660] Mountpoint-cache hash table entries: 2048 (order: 1, 8192 bytes)
[    0.001666] Disabling memory control group subsystem
[    0.001738] CPU: Testing write buffer coherency: ok
[    0.001772] ftrace: allocating 22392 entries in 66 pages
[    0.048823] CPU0: update cpu_capacity 1024
[    0.048838] CPU0: thread -1, cpu 0, socket 0, mpidr 80000000
[    0.048874] Setting up static identity map for 0x100000 - 0x100034
[    0.050733] CPU1: update cpu_capacity 1024
[    0.050740] CPU1: thread -1, cpu 1, socket 0, mpidr 80000001
[    0.051425] CPU2: update cpu_capacity 1024
[    0.051432] CPU2: thread -1, cpu 2, socket 0, mpidr 80000002
[    0.052101] CPU3: update cpu_capacity 1024
[    0.052108] CPU3: thread -1, cpu 3, socket 0, mpidr 80000003
[    0.052195] Brought up 4 CPUs
[    0.052205] SMP: Total of 4 processors activated (153.60 BogoMIPS).
[    0.052209] CPU: All CPU(s) started in HYP mode.
[    0.052213] CPU: Virtualization extensions available.
[    0.053007] devtmpfs: initialized
[    0.064440] VFP support v0.3: implementor 41 architecture 3 part 40 variant 3 rev 4
[    0.064710] clocksource: jiffies: mask: 0xffffffff max_cycles: 0xffffffff, max_idle_ns: 19112604462750000 ns
[    0.064726] futex hash table entries: 1024 (order: 4, 65536 bytes)
[    0.065262] pinctrl core: initialized pinctrl subsystem
[    0.066168] NET: Registered protocol family 16
[    0.068513] DMA: preallocated 1024 KiB pool for atomic coherent allocations
[    0.077460] hw-breakpoint: found 5 (+1 reserved) breakpoint and 4 watchpoint registers.
[    0.077466] hw-breakpoint: maximum watchpoint size is 8 bytes.
[    0.077605] Serial: AMBA PL011 UART driver
[    0.079507] bcm2835-mbox 3f00b880.mailbox: mailbox enabled
[    0.080031] uart-pl011 3f201000.serial: could not find pctldev for node /soc/gpio@7e200000/uart0_pins, deferring probe
[    0.149657] bcm2835-dma 3f007000.dma: DMA legacy API manager at bb80f000, dmachans=0x1
[    0.151473] SCSI subsystem initialized
[    0.151623] usbcore: registered new interface driver usbfs
[    0.151699] usbcore: registered new interface driver hub
[    0.151789] usbcore: registered new device driver usb
[    0.158627] raspberrypi-firmware soc:firmware: Attached to firmware from 2017-10-24 17:09
[    0.160101] clocksource: Switched to clocksource arch_sys_counter
[    0.207117] VFS: Disk quotas dquot_6.6.0
[    0.207193] VFS: Dquot-cache hash table entries: 1024 (order 0, 4096 bytes)
[    0.207395] FS-Cache: Loaded
[    0.207643] CacheFiles: Loaded
[    0.219765] NET: Registered protocol family 2
[    0.220663] TCP established hash table entries: 8192 (order: 3, 32768 bytes)
[    0.220770] TCP bind hash table entries: 8192 (order: 4, 65536 bytes)
[    0.220955] TCP: Hash tables configured (established 8192 bind 8192)
[    0.221042] UDP hash table entries: 512 (order: 2, 16384 bytes)
[    0.221084] UDP-Lite hash table entries: 512 (order: 2, 16384 bytes)
[    0.221288] NET: Registered protocol family 1
[    0.221694] RPC: Registered named UNIX socket transport module.
[    0.221699] RPC: Registered udp transport module.
[    0.221704] RPC: Registered tcp transport module.
[    0.221708] RPC: Registered tcp NFSv4.1 backchannel transport module.
[    0.222760] hw perfevents: enabled with armv7_cortex_a7 PMU driver, 7 counters available
[    0.225051] workingset: timestamp_bits=14 max_order=18 bucket_order=4
[    0.241107] FS-Cache: Netfs 'nfs' registered for caching
[    0.242080] NFS: Registering the id_resolver key type
[    0.242106] Key type id_resolver registered
[    0.242111] Key type id_legacy registered
[    0.244498] Block layer SCSI generic (bsg) driver version 0.4 loaded (major 251)
[    0.244600] io scheduler noop registered
[    0.244606] io scheduler deadline registered (default)
[    0.244876] io scheduler cfq registered
[    0.250509] BCM2708FB: allocated DMA memory fad10000
[    0.250532] BCM2708FB: allocated DMA channel 0 @ bb80f000
[    0.280246] Console: switching to colour frame buffer device 170x48
[    0.298482] bcm2835-rng 3f104000.rng: hwrng registered
[    0.298598] vc-mem: phys_addr:0x00000000 mem_base=0x3ec00000 mem_size:0x40000000(1024 MiB)
[    0.299124] vc-sm: Videocore shared memory driver
[    0.314280] brd: module loaded
[    0.323216] loop: module loaded
[    0.323227] Loading iSCSI transport class v2.0-870.
[    0.323765] usbcore: registered new interface driver smsc95xx
[    0.323780] dwc_otg: version 3.00a 10-AUG-2012 (platform bus)
[    0.551842] Core Release: 2.80a
[    0.551850] Setting default values for core params
[    0.551882] Finished setting default values for core params
[    0.752269] Using Buffer DMA mode
[    0.752275] Periodic Transfer Interrupt Enhancement - disabled
[    0.752279] Multiprocessor Interrupt Enhancement - disabled
[    0.752285] OTG VER PARAM: 0, OTG VER FLAG: 0
[    0.752299] Dedicated Tx FIFOs mode
[    0.752662] WARN::dwc_otg_hcd_init:1032: FIQ DMA bounce buffers: virt = 0xbad04000 dma = 0xfad04000 len=9024
[    0.752687] FIQ FSM acceleration enabled for :
               Non-periodic Split Transactions
               Periodic Split Transactions
               High-Speed Isochronous Endpoints
               Interrupt/Control Split Transaction hack enabled
[    0.752694] dwc_otg: Microframe scheduler enabled
[    0.752740] WARN::hcd_init_fiq:459: FIQ on core 1 at 0x8058f5b0
[    0.752750] WARN::hcd_init_fiq:460: FIQ ASM at 0x8058f920 length 36
[    0.752761] WARN::hcd_init_fiq:486: MPHI regs_base at 0xbb87a000
[    0.752822] dwc_otg 3f980000.usb: DWC OTG Controller
[    0.752855] dwc_otg 3f980000.usb: new USB bus registered, assigned bus number 1
[    0.752885] dwc_otg 3f980000.usb: irq 62, io mem 0x00000000
[    0.752933] Init: Port Power? op_state=1
[    0.752938] Init: Power Port (0)
[    0.753150] usb usb1: New USB device found, idVendor=1d6b, idProduct=0002
[    0.753160] usb usb1: New USB device strings: Mfr=3, Product=2, SerialNumber=1
[    0.753169] usb usb1: Product: DWC OTG Controller
[    0.753176] usb usb1: Manufacturer: Linux 4.9.59-v7+ dwc_otg_hcd
[    0.753184] usb usb1: SerialNumber: 3f980000.usb
[    0.754005] hub 1-0:1.0: USB hub found
[    0.754042] hub 1-0:1.0: 1 port detected
[    0.754735] dwc_otg: FIQ enabled
[    0.754739] dwc_otg: NAK holdoff enabled
[    0.754743] dwc_otg: FIQ split-transaction FSM enabled
[    0.754756] Module dwc_common_port init
[    0.754980] usbcore: registered new interface driver usb-storage
[    0.755225] mousedev: PS/2 mouse device common for all mice
[    0.756204] bcm2835-wdt 3f100000.watchdog: Broadcom BCM2835 watchdog timer
[    0.756477] bcm2835-cpufreq: min=600000 max=1200000
[    0.756863] sdhci: Secure Digital Host Controller Interface driver
[    0.756867] sdhci: Copyright(c) Pierre Ossman
[    0.757145] sdhost-bcm2835 3f202000.sdhost: could not get clk, deferring probe
[    0.759318] mmc-bcm2835 3f300000.mmc: could not get clk, deferring probe
[    0.759417] sdhci-pltfm: SDHCI platform and OF driver helper
[    0.762041] ledtrig-cpu: registered to indicate activity on CPUs
[    0.762230] hidraw: raw HID events driver (C) Jiri Kosina
[    0.762418] usbcore: registered new interface driver usbhid
[    0.762422] usbhid: USB HID core driver
[    0.763214] vchiq: vchiq_init_state: slot_zero = 0xbad80000, is_master = 0
[    0.764882] [vc_sm_connected_init]: start
[    0.773847] [vc_sm_connected_init]: end - returning 0
[    0.774205] Initializing XFRM netlink socket
[    0.774227] NET: Registered protocol family 17
[    0.774346] Key type dns_resolver registered
[    0.774848] Registering SWP/SWPB emulation handler
[    0.775530] registered taskstats version 1
[    0.781796] uart-pl011 3f201000.serial: cts_event_workaround enabled
[    0.781866] 3f201000.serial: ttyAMA0 at MMIO 0x3f201000 (irq = 87, base_baud = 0) is a PL011 rev2
[    0.783439] sdhost: log_buf @ bad07000 (fad07000)
[    0.860135] mmc0: sdhost-bcm2835 loaded - DMA enabled (>1)
[    0.862350] mmc-bcm2835 3f300000.mmc: mmc_debug:0 mmc_debug2:0
[    0.862358] mmc-bcm2835 3f300000.mmc: DMA channel allocated
[    0.920237] of_cfs_init
[    0.920457] of_cfs_init: OK
[    0.920954] Waiting for root device PARTUUID=00aa1cb9-02...
[    0.930893] mmc0: host does not support reading read-only switch, assuming write-enable
[    0.932905] mmc0: new high speed SDHC card at address 1234
[    0.933570] mmcblk0: mmc0:1234 SA08G 7.25 GiB
[    0.935138]  mmcblk0: p1 p2
[    0.941242] mmc1: queuing unknown CIS tuple 0x80 (2 bytes)
[    0.942790] mmc1: queuing unknown CIS tuple 0x80 (3 bytes)
[    0.944337] mmc1: queuing unknown CIS tuple 0x80 (3 bytes)
[    0.947116] mmc1: queuing unknown CIS tuple 0x80 (7 bytes)
[    0.970206] Indeed it is in host mode hprt0 = 00021501
[    1.037745] random: fast init done
[    1.054005] EXT4-fs (mmcblk0p2): mounted filesystem with ordered data mode. Opts: (null)
[    1.054052] VFS: Mounted root (ext4 filesystem) readonly on device 179:2.
[    1.055188] devtmpfs: mounted
[    1.057039] Freeing unused kernel memory: 1024K
[    1.098350] mmc1: new high speed SDIO card at address 0001
[    1.170155] usb 1-1: new high-speed USB device number 2 using dwc_otg
[    1.170296] Indeed it is in host mode hprt0 = 00001101
[    1.400477] usb 1-1: New USB device found, idVendor=0424, idProduct=9514
[    1.400492] usb 1-1: New USB device strings: Mfr=0, Product=0, SerialNumber=0
[    1.401330] hub 1-1:1.0: USB hub found
[    1.401425] hub 1-1:1.0: 5 ports detected
[    1.513692] systemd[1]: System time before build time, advancing clock.
[    1.642640] NET: Registered protocol family 10
[    1.663074] ip_tables: (C) 2000-2006 Netfilter Core Team
[    1.687567] systemd[1]: systemd 232 running in system mode. (+PAM +AUDIT +SELINUX +IMA +APPARMOR +SMACK +SYSVINIT +UTMP +LIBCRYPTSETUP +GCRYPT +GNUTLS +ACL +XZ +LZ4 +SECCOMP +BLKID +ELFUTILS +KMOD +IDN)
[    1.688138] systemd[1]: Detected architecture arm.
[    1.689287] systemd[1]: Set hostname to <raspberrypi>.
[    1.720166] usb 1-1.1: new high-speed USB device number 3 using dwc_otg
[    1.850490] usb 1-1.1: New USB device found, idVendor=0424, idProduct=ec00
[    1.850505] usb 1-1.1: New USB device strings: Mfr=0, Product=0, SerialNumber=0
[    1.853314] smsc95xx v1.0.5
[    1.944109] smsc95xx 1-1.1:1.0 eth0: register 'smsc95xx' at usb-3f980000.usb-1.1, smsc95xx USB 2.0 Ethernet, b8:27:eb:68:da:f4
[    2.040152] usb 1-1.3: new high-speed USB device number 4 using dwc_otg
[    2.168270] systemd[1]: Listening on Journal Socket (/dev/log).
[    2.169368] systemd[1]: Set up automount Arbitrary Executable File Formats File System Automount Point.
[    2.169674] systemd[1]: Listening on Journal Socket.
[    2.171571] usb 1-1.3: New USB device found, idVendor=05e3, idProduct=0608
[    2.171585] usb 1-1.3: New USB device strings: Mfr=0, Product=1, SerialNumber=0
[    2.171594] usb 1-1.3: Product: USB2.0 Hub
[    2.172514] hub 1-1.3:1.0: USB hub found
[    2.172812] hub 1-1.3:1.0: 4 ports detected
[    2.189392] systemd[1]: Listening on fsck to fsckd communication Socket.
[    2.189656] systemd[1]: Listening on udev Kernel Socket.
[    2.189910] systemd[1]: Listening on udev Control Socket.
[    2.190758] systemd[1]: Created slice User and Session Slice.
[    2.313707] i2c /dev entries driver
[    2.490176] usb 1-1.3.3: new low-speed USB device number 5 using dwc_otg
[    2.626572] usb 1-1.3.3: New USB device found, idVendor=046d, idProduct=c05a
[    2.626589] usb 1-1.3.3: New USB device strings: Mfr=1, Product=2, SerialNumber=0
[    2.626598] usb 1-1.3.3: Product: USB Optical Mouse
[    2.626605] usb 1-1.3.3: Manufacturer: Logitech
[    2.635785] input: Logitech USB Optical Mouse as /devices/platform/soc/3f980000.usb/usb1/1-1/1-1.3/1-1.3.3/1-1.3.3:1.0/0003:046D:C05A.0001/input/input0
[    2.636388] hid-generic 0003:046D:C05A.0001: input,hidraw0: USB HID v1.11 Mouse [Logitech USB Optical Mouse] on usb-3f980000.usb-1.3.3/input0
[    2.730149] usb 1-1.3.4: new low-speed USB device number 6 using dwc_otg
[    2.762728] EXT4-fs (mmcblk0p2): re-mounted. Opts: (null)
[    2.867026] systemd-journald[118]: Received request to flush runtime journal from PID 1
[    2.871226] usb 1-1.3.4: New USB device found, idVendor=046d, idProduct=c31c
[    2.871244] usb 1-1.3.4: New USB device strings: Mfr=1, Product=2, SerialNumber=0
[    2.871260] usb 1-1.3.4: Product: USB Keyboard
[    2.871267] usb 1-1.3.4: Manufacturer: Logitech
[    2.886091] input: Logitech USB Keyboard as /devices/platform/soc/3f980000.usb/usb1/1-1/1-1.3/1-1.3.4/1-1.3.4:1.0/0003:046D:C31C.0002/input/input1
[    2.952917] hid-generic 0003:046D:C31C.0002: input,hidraw1: USB HID v1.10 Keyboard [Logitech USB Keyboard] on usb-3f980000.usb-1.3.4/input0
[    2.969956] input: Logitech USB Keyboard as /devices/platform/soc/3f980000.usb/usb1/1-1/1-1.3/1-1.3.4/1-1.3.4:1.1/0003:046D:C31C.0003/input/input2
[    3.030620] hid-generic 0003:046D:C31C.0003: input,hidraw2: USB HID v1.10 Device [Logitech USB Keyboard] on usb-3f980000.usb-1.3.4/input1
[    3.524055] gpiomem-bcm2835 3f200000.gpiomem: Initialised: Registers at 0x3f200000
[    3.830958] brcmfmac: F1 signature read @0x18000000=0x1541a9a6
[    3.838058] usbcore: registered new interface driver brcmfmac
[    4.045867] brcmfmac: Firmware version = wl0: Aug  7 2017 00:46:29 version 7.45.41.46 (r666254 CY) FWID 01-f8a78378
[    4.046831] brcmfmac: brcmf_c_preinit_dcmds: CLM version = API: 12.2 Data: 7.11.15 Compiler: 1.24.2 ClmImport: 1.24.1 Creation: 2014-05-26 10:53:55 Inc Data: 9.10.41 Inc Compiler: 1.29.4 Inc ClmImport: 1.36.3 Creation: 2017-08-07 00:37:47 
[    4.942461] uart-pl011 3f201000.serial: no DMA platform data
[    5.455926] IPv6: ADDRCONF(NETDEV_UP): wlan0: link is not ready
[    5.456093] brcmfmac: power management disabled
[    5.852483] smsc95xx 1-1.1:1.0 eth0: hardware isn't capable of remote wakeup
[    5.852721] IPv6: ADDRCONF(NETDEV_UP): eth0: link is not ready
[    6.476707] Adding 102396k swap on /var/swap.  Priority:-1 extents:1 across:102396k SSFS
[    7.375104] IPv6: ADDRCONF(NETDEV_CHANGE): eth0: link becomes ready
[    7.375800] smsc95xx 1-1.1:1.0 eth0: link up, 100Mbps, full-duplex, lpa 0xC5E1
[    9.438277] Bluetooth: Core ver 2.22
[    9.438365] NET: Registered protocol family 31
[    9.438368] Bluetooth: HCI device and connection manager initialized
[    9.439211] Bluetooth: HCI socket layer initialized
[    9.439221] Bluetooth: L2CAP socket layer initialized
[    9.439247] Bluetooth: SCO socket layer initialized
[    9.461150] Bluetooth: HCI UART driver ver 2.3
[    9.461157] Bluetooth: HCI UART protocol H4 registered
[    9.461160] Bluetooth: HCI UART protocol Three-wire (H5) registered
[    9.461253] Bluetooth: HCI UART protocol Broadcom registered
[    9.689939] Bluetooth: BNEP (Ethernet Emulation) ver 1.3
[    9.689948] Bluetooth: BNEP filters: protocol multicast
[    9.689963] Bluetooth: BNEP socket layer initialized
[    9.748062] Bluetooth: RFCOMM TTY layer initialized
[    9.748090] Bluetooth: RFCOMM socket layer initialized
[    9.748110] Bluetooth: RFCOMM ver 1.11
[   12.936040] fuse init (API version 7.26)
[   19.839955] random: crng init done
[   38.486026] usb 1-1.3: USB disconnect, device number 4
[   38.486042] usb 1-1.3.3: USB disconnect, device number 5
[   38.561228] usb 1-1.3.4: USB disconnect, device number 6
[   68.220200] usb 1-1.3: new high-speed USB device number 7 using dwc_otg
[   68.351618] usb 1-1.3: New USB device found, idVendor=05e3, idProduct=0608
[   68.351634] usb 1-1.3: New USB device strings: Mfr=0, Product=1, SerialNumber=0
[   68.351643] usb 1-1.3: Product: USB2.0 Hub
[   68.354864] hub 1-1.3:1.0: USB hub found
[   68.355903] hub 1-1.3:1.0: 4 ports detected
[   68.670157] usb 1-1.3.3: new low-speed USB device number 8 using dwc_otg
[   68.806549] usb 1-1.3.3: New USB device found, idVendor=046d, idProduct=c05a
[   68.806562] usb 1-1.3.3: New USB device strings: Mfr=1, Product=2, SerialNumber=0
[   68.806571] usb 1-1.3.3: Product: USB Optical Mouse
[   68.806578] usb 1-1.3.3: Manufacturer: Logitech
[   68.814213] input: Logitech USB Optical Mouse as /devices/platform/soc/3f980000.usb/usb1/1-1/1-1.3/1-1.3.3/1-1.3.3:1.0/0003:046D:C05A.0004/input/input3
[   68.817549] hid-generic 0003:046D:C05A.0004: input,hidraw0: USB HID v1.11 Mouse [Logitech USB Optical Mouse] on usb-3f980000.usb-1.3.3/input0
[   68.910142] usb 1-1.3.4: new low-speed USB device number 9 using dwc_otg
[   69.067151] usb 1-1.3.4: New USB device found, idVendor=046d, idProduct=c31c
[   69.067160] usb 1-1.3.4: New USB device strings: Mfr=1, Product=2, SerialNumber=0
[   69.067164] usb 1-1.3.4: Product: USB Keyboard
[   69.067168] usb 1-1.3.4: Manufacturer: Logitech
[   69.080191] input: Logitech USB Keyboard as /devices/platform/soc/3f980000.usb/usb1/1-1/1-1.3/1-1.3.4/1-1.3.4:1.0/0003:046D:C31C.0005/input/input4
[   69.150865] hid-generic 0003:046D:C31C.0005: input,hidraw1: USB HID v1.10 Keyboard [Logitech USB Keyboard] on usb-3f980000.usb-1.3.4/input0
[   69.161267] input: Logitech USB Keyboard as /devices/platform/soc/3f980000.usb/usb1/1-1/1-1.3/1-1.3.4/1-1.3.4:1.1/0003:046D:C31C.0006/input/input5
[   69.230424] hid-generic 0003:046D:C31C.0006: input,hidraw2: USB HID v1.10 Device [Logitech USB Keyboard] on usb-3f980000.usb-1.3.4/input1
[   78.422006] usb 1-1.3: USB disconnect, device number 7
[   78.422022] usb 1-1.3.3: USB disconnect, device number 8
[   78.531158] usb 1-1.3.4: USB disconnect, device number 9
[   96.382524] usb 1-1.5: new high-speed USB device number 10 using dwc_otg
[   96.514068] usb 1-1.5: New USB device found, idVendor=05e3, idProduct=0608
[   96.514082] usb 1-1.5: New USB device strings: Mfr=0, Product=1, SerialNumber=0
[   96.514092] usb 1-1.5: Product: USB2.0 Hub
[   96.515103] hub 1-1.5:1.0: USB hub found
[   96.515435] hub 1-1.5:1.0: 4 ports detected
[   96.832634] usb 1-1.5.3: new low-speed USB device number 11 using dwc_otg
[   96.969046] usb 1-1.5.3: New USB device found, idVendor=046d, idProduct=c05a
[   96.969059] usb 1-1.5.3: New USB device strings: Mfr=1, Product=2, SerialNumber=0
[   96.969068] usb 1-1.5.3: Product: USB Optical Mouse
[   96.969075] usb 1-1.5.3: Manufacturer: Logitech
[   96.975182] input: Logitech USB Optical Mouse as /devices/platform/soc/3f980000.usb/usb1/1-1/1-1.5/1-1.5.3/1-1.5.3:1.0/0003:046D:C05A.0007/input/input6
[   96.975942] hid-generic 0003:046D:C05A.0007: input,hidraw0: USB HID v1.11 Mouse [Logitech USB Optical Mouse] on usb-3f980000.usb-1.5.3/input0
[   97.072794] usb 1-1.5.4: new low-speed USB device number 12 using dwc_otg
[   97.216553] usb 1-1.5.4: New USB device found, idVendor=046d, idProduct=c31c
[   97.216569] usb 1-1.5.4: New USB device strings: Mfr=1, Product=2, SerialNumber=0
[   97.216577] usb 1-1.5.4: Product: USB Keyboard
[   97.216585] usb 1-1.5.4: Manufacturer: Logitech
[   97.225618] input: Logitech USB Keyboard as /devices/platform/soc/3f980000.usb/usb1/1-1/1-1.5/1-1.5.4/1-1.5.4:1.0/0003:046D:C31C.0008/input/input7
[   97.294270] hid-generic 0003:046D:C31C.0008: input,hidraw1: USB HID v1.10 Keyboard [Logitech USB Keyboard] on usb-3f980000.usb-1.5.4/input0
[   97.309427] input: Logitech USB Keyboard as /devices/platform/soc/3f980000.usb/usb1/1-1/1-1.5/1-1.5.4/1-1.5.4:1.1/0003:046D:C31C.0009/input/input8
[   97.373251] hid-generic 0003:046D:C31C.0009: input,hidraw2: USB HID v1.10 Device [Logitech USB Keyboard] on usb-3f980000.usb-1.5.4/input1
pi@raspberrypi:~ $ 
```
