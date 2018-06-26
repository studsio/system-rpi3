# Changelog

#### Version 1.3 (working)
* Upgraded the Linux kernel from 4.4 -> 4.9
* Rename `roofts-additions` -> `rootfs_overlay`
* Support for the Raspberry Pi Compute Module
* Select ARM Cortex A53 as CPU for Buildroot
* Disable console blanking for HDMI to make it easier to capture error messages
* Support for reverting firmware
* Support for Raspberry Pi 3 B+
* The serial port on the GPIO pins is now assigned to "dev/ttyAMA0" like all other RPi systems
* Add global patch directory
    - This is required to pull in the e2fsprogs patch that's needed now that
      util-linux's uuid_generate function calls getrandom and can block
      indefinitely for the urandom pool to initialize
* Buildroot 2017.11
* Toolchains 1.0.0
* nbtty 0.3.0

#### Version 1.2 (29-Nov-2017)
* Remove Erlang/erlinit/Exilir depends
* fwup.conf improvements

#### Version 1.1 (15-Aug-2017)
* Fork from nerves_system_rpi3
* Buildroot 2017.05
* Bump Linux kernel to 4.4.50
* Bump toolchain to use gcc 5.3 (previously using gcc 4.9.3)
* Bump fwup to 0.15.3
* Increased GPU memory to support Pi Camera V2
* The application data partition is now `ext4`

#### Version 1.0
Duplicate nerves-system-rpi3 image
