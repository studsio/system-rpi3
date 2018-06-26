# Changelog

#### Version 1.3 (working)
* Rename `roofts-additions` -> `rootfs_overlay`
* Support for the Raspberry Pi Compute Module
* Select ARM Cortex A53 as CPU for Buildroot
* Buildroot 2017.08
* Toolchains 0.12.1
* fwup 0.17.0
* nbtty 0.3.0
* Add global patch directory (required to pull in the e2fsprogs patch that's
  needed now that util-linux's uuid_generate function calls getrandom and can
  block indefinitely for the urandom pool to initialize)

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
