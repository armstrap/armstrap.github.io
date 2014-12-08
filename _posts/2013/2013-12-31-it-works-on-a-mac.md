---
layout: post
title:  "It Works on a MAC"
---

![ARMstrap on a MAc](/img/posts/2013/12/armstrap-mac-featured.jpg)

Quarter by quarter, news outlets are reporting that [PC sales are either flat][1] or plummeting.  HP just announced [another layoff][2] in an on-going effort to restructure and reinvent themselves.  Dell went as far as to [convert themselves to a private company][3].  Since we are not in an economic depression, all of these articles hint at one fundamental fact–Mac sales are rising.

When I look at the options embedded developers have on the Mac, the outcome is grim.  External JTAG devices require a proprietary driver to enumerate and those JTAG vendors only ship drivers for the PC.  That shiny new MacBook Pro can’t do any real-world embedded development without a lot of hackery.  It’s no wonder that products like the [BeagleBone Black][4] and the [Raspberry Pi][5] exist.  It’s easier to put an entire operating system on a chip than to create a new driver stack for a different ecosystem, [riddled with lawyers][6] and politics.  No drivers are required when your embedded board ships with an entire operating system on board.  But what happens to those developers who want to be close to the hardware?  These developers don’t want an operating system in the way of their time-critical projects.

ARMstrap is different.

**ARMstrap boards don’t abstract away the hardware, they embrace it.**  Rather than putting a TCP/IP between your code and the hardware, ARMstrap boards connect to your project directly via a standard USB cable.  There are no external adapters to worry about.  Debugging is done on any platform (Windows, Mac or Linux) because ARMstrap boards enumerate as a tty serial device, utilizing the standard USB driver stack.  Debugging is ultra fast and snappy thanks to the heavy lifting done by the open source debugger that comes integrated on every ARMstrap board.

Finally, ARM development that actually works on a Mac.

[1]: http://www.pcmag.com/article2/0,2817,2417655,00.asp
[2]: http://www.pcmag.com/article2/0,2817,2428865,00.asp
[3]: http://www.forbes.com/sites/connieguglielmo/2013/10/30/you-wont-have-michael-dell-to-kick-around-anymore/
[4]: http://beagleboard.org/products/beaglebone%20black
[5]: http://www.raspberrypi.org/
[6]: http://www.apple.com/legal/macapps/stdeula/