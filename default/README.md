This `preseed.cfg` automatically installs the entire system and updates `/etc/apt/sources.list` on the new system with a `sources.list` file (included in this directory) that uses `https`.

The addition of the `nomodeset systemd.unit=multi-user.target` parameters to `/etc/default/grub` allows for running a console-only Debian environment through Qemu's `-curses` flag, e.g.

    qemu-system-x86_64 -curses -vga std -m 1024 -drive format=raw,file=disk.img
