# uImage-eselect
Eselect module to manage /boot/uImage symlink.
Intended for embedded devices with uboot or similarily trivial bootloader.
Configure bootloader to point to /boot/uImage instead of a specific kernel version.
Manage kernel for next boot through `eselect uImage set <n>` command.
Only lists uImage binaries found in /boot/uImage-[[:digit:]]*

Install to /usr/share/eselect/modules/.

#### Example output:
```console
$ eselect uImage list
Available uImage symlink targets:
  [1]   uImage-5.8.1-gentoo
  [2]   uImage-5.8.2-gentoo
  [3]   uImage-5.8.3-gentoo *
```
