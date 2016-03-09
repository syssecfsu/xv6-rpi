# Project description #
[Xv6](http://pdos.csail.mit.edu/6.828/2012/xv6.html) is a simple Unix-like teaching operating system developed in 2006 by MIT for its operating system course. Xv6 is inspired by and modeled after the Sixth Edition Unix (aka V6). Xv6 is fairly complete educational operating system while remaining simply and manageable. It has most components in an early Unix system, such as processes, virtual memory, kernel-user separation, interrupt, file system...

The original xv6 is implemented for the x86 architecture. This is an effort to port xv6 to ARM, particularly [Raspberry Pi](http://www.raspberrypi.org/). The initial porting of xv6 to ARM (QEMU/ARMv6) has been completed by people in the department of [computer science](http://www.cs.fsu.edu) in [Florida State University](http://www.fsu.edu).

# Current status #
  * Most part of xv6 has been ported to Raspberry Pi. It can successfully boot to the shell. The current work-in-progress is accessible in the rpi branch of the source tree.

This is a picture of [xv6 running in shell](http://xv6-rpi.googlecode.com/files/shell.jpg).

# What to do #
  * Add USB keyboard support
  * Enhance the kernel memory allocator. The original kernel memory allocator uses linked list for free memory management. A buddy allocator for page allocation, and a simple slab allocator for smaller-sized memory allocation would be nice.
  * More hardware support, particularly the flash memory.
  * A virtual file system interface.
  * FAT32/FAT16 file system.
  * More system calls.
  * Networking (Ethernet/socket/TCP/IP) such as [lwIP](http://savannah.nongnu.org/projects/lwip/)
  * Documentation, to help others get started and understand the internal working of the OS.

If you would like to become a project member, please contact [Zhi Wang](http://www.cs.fsu.edu/~zwang/). Your contributed code need to be licensed in MIT license.