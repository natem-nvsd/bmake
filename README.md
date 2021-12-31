bmake
=====

This directory contains a port of the BSD make tool (from NetBSD).
Since 1993 I have run it on AIX, BSDi, Darwin, FreeBSD, HP-UX, IRIX,
Linux, Minix, OSF, Solaris, SunOS and even UTS.
Others have run it on many more systems.

Currently each release is tested on NetBSD, FreeBSD, Solaris and Linux.

Since 2003 bmake switched to a date based version (first was 20030714)
which generally represents the date it was last merged with NetBSD's
make.  Since then, NetBSD's make is imported within a week of any
interesting changes, so that bmake tracks it very closely.

Building
========

The preferred way to bootstrap bmake is::

	./bmake/boot-strap

there are a number of args - most of which get passed to configure,
eg.
::

	./bmake/boot-strap --prefix=/opt

see the boot-strap script for details.

For folk that hate to read anything, since 20121212 you can also use
the GNU standard process of::

	./configure; make; make install

To make much use of bmake you will need the bsd.*.mk macros or my
portable *.mk macros which are included with bmake since 20121212
and separately available from
http://www.crufty.net/ftp/pub/sjg/mk.tar.gz
which will be links to the latest versions.

Porting
=======

If you encounter a system that bmake does not build or work on *out of
the box*, I welcome patches.
If you can provide access to a suitable machine - even better.

More info can be found at http://www.crufty.net/help/sjg/bmake.htm

--sjg <sjg@crufty.net>

