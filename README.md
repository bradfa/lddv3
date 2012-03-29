# Linux Device Drivers, 3rd Edition

This repo contains code examples that I've created while reading through [Linux
Device Drivers, 3rd Edition][1].

All examples are built against [Linux version 3.0][2] and run on a Debian
GNU/Linux 6 Squeeze x86_64 virtual machine within [VirtualBox][3] using 2
processor cores.  My kernel config is the x86_64_defconfig with only a minor
change (enabling devtmpfs via menuconfig to avoid needing initramfs).  Building
against a patched 3.0.y kernel should also work.

Each chapter is broken into its own directory.  To build, use the provided
Makefile in each directory and be sure to supply a KERNELDIR value that points
to your local copy of the Linux 3.0 source where you have built a kernel (this
last point, that you must have built a kernel, is very important).

[1]: http://www.amazon.com/gp/product/0596005903/ref=as_li_ss_tl?ie=UTF8&tag=bradford07-20&linkCode=as2&camp=1789&creative=390957&creativeASIN=0596005903
[2]: ftp://ftp.kernel.org/pub/linux/kernel/v3.x/linux-3.0.tar.gz
[3]: https://www.virtualbox.org/

