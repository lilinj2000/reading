Chapter 5. Network Device Initialization

- 5.1 System Initialization Overview

  - Boot-time options
  - Interrupts and timers
  - Initialization routines

- 5.2 Device Registration and Initialization

  - Hardware initialization
  - Software initialization
  - Feature initialization

- 5.3 Basic Goals of NIC Initialization

  - IRQ line
  - I/O ports and memory registration

- 5.4 Interaction Between Devices and Kernel

  Polling: Driven on the kernel side.
  Interrupt: Driven on the device side​

  - 5.4.1 Hardware Interrupts
  - 5.4.1.1 Interrupt types
    - Reception of a frame
    - Transmission failure
    - DMA transfer has completed successfully
    - Device has enough memory to handle a new transmission
  - 5.4.1.2 Interrupt sharing
  - 5.4.1.3 Organization of IRSs to handler mappings

- 5.5 Initialization Options

  - Module options
  - Boot-time kernel options

- 5.6 Module Options

- 5.7 Initializing the Device Handling Layer: net_dev_init

  - 5.7.1 Legacy Code

- 5.8 User-Space Helpers

  /sbin/modprobe
  /sbin/hotplug​

  - 5.8.1 kmod
  - 5.8.2 Hotplug
    - 5.8.2.1 /sbin/hotplug

- 5.9 Virtual Devices

  - 5.9.1 Examples of Virtual Devices
    - Bonding
    - 802.1Q
    - Bridging
    - Aliasing interfaces
    - True equalizer(TEQL)
    - Tunnel interfaces
  - 5.9.2 Interaction with the Kernel Network Stack

- 5.10 Tuning via /proc Filesystem

- 5.11 Functions and Variables Featured in This Chapter

- 5.12 Files and Directories Featured in This Chapter