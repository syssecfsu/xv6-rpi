# Introduction #

The initial release of xv6 for ARM has, so far, only been tested with Mac OSX 10.8.2 as the development host (though it should be straight-forward to support the Linux host).


# Details #
Here are the steps to build and run xv6 for ARM:
  * Install [MacPorts](http://www.macports.org/)
  * Install the cross-compiler arm-none-eabi-gcc, git, and qemu-system-arm with MacPorts.
  * Clone the xv6 for ARM source code:
> > `git clone https://xv6rpi@code.google.com/p/xv6-rpi/`
  * execute the following command in the root of the source code:
> > `make qemu`


> It should build the OS and run it in QEMU.