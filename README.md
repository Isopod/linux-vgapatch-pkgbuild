# linux-kvmvga-pkgbuild
This is an Arch Linux PKGBUILD for a kernel based on Linux Mainline v4.1, patched for better VGA passthrough compatibility. Use at your own risk!

It includes the following patches by Alex Williamson:
- [i915: Add module option to support VGA arbiter on HD devices](https://lkml.org/lkml/2014/5/9/517)
- [pci: Enable overrides for missing ACS capabilities](https://lkml.org/lkml/2013/5/30/513)

Note: This only saves you the trouble of patching your kernel. In addition to installing this kernel, you will still need to edit your mkinitcpio.conf and your grub config. For more detailed instructions, here are some good resources:
- https://bbs.archlinux.org/viewtopic.php?id=162768
- http://vfio.blogspot.de/
