---
layout: page
title: Core Values
permalink: /core-values/
---

![Community](/img/pages/online-community.jpg){: .centered .img-responsive}

# Why does ARMstrap Exist?

**ARM development and debugging is too hard.**  It's too hard because the tools used to develop and debug ARM boards are too hard and too expensive to use.  ARMstrap is a open-source community that's going to change all of that.

Here are the core values that we live by to make ARM development easy, open and fun.

1. Integrated JTAG
2. Multi-Platform Toolchain and IDE
3. Open Source
4. Remixable


## Integrated JTAG

A JTAG device is a critical element required to do effective ARM development.  This device is used to flash and debug your ARM chip.  It's usually an external device that attaches to your development board and relies on a proprietary driver to operate successfully.

**ARMstrap development boards build the JTAG device into the development board**, allowing developers to worry about more important things--like their code.  External JTAG devices are awful.  It's yet another device on an engineer's cluttered desk that cannot be found when it's needed.  There are also [several JTAG interfacing standards][1].  You'll likely [need an adapter][2] to convert from one connector type (the one that came with your JTAG device) to another (the one that's on your project's board).  These adapters often get lost or misplaced when developers move from project to project.  Fixing even the most trivial firmware bug after release becomes incredibly expensive.

**The integrated JTAG on ARMstrap development boards work on every operating system.**  Closed JTAG devices ship with closed-source drivers.  Those drivers couple your development to a particular operating system.  Changing your development environment (whether upgrading to a newer operating system, or changing ecosystems) is non-trivial because of driver compatibility issues.  **ARMstrap development board enumerates as a standard USB serial device**, meaning you are not handcuffed to a particular operating system or ecosystem.  Developers can start their project on a Microsoft Windows platform and move to Mac or Linux whenever they wish.  This alleviates many headaches during development and makes ARM development easy.

Also, many expensive JTAG debuggers come riddled with DRM features, such as a size-limit on your final binary or a limit on how many breakpoints you can set during debugging.  When hitting a size-limit boundary, developers have to resort to awful workarounds because they don't have the time or money to upgrade their device.  **The integrated JTAG on ARMstrap development board have no hardware crippling features.**

## Multi-Platform Toolchain and IDE

A multi-platform integrated development environment (IDE) and toolchain are important for effective ARM development.  Their function is to house your code and provide tools to help development--like tools to debug your code via the JTAG debugger.  IDEs are really hard to get right and its unfortunate that many toolchain vendors insist on using their expensive DRM-riddle IDE.

**ARMstrap development relies on the open source "Eclipse" IDE, specifically configured for ARM development.**  Eclipse has some of the best advanced features that real-world developers know and depend on to make development productive.  Developers can easily write code, flash their chip, debug and inspect variables at runtime, without any compromises or headaches.  **ARMstrap Eclipse comes pre-configured with the [GNU Tools for ARM Embedded Processors][3] that works with Mac, Linux and Windows.**.  There are no licenses to worry about, and there are no serial USB keys to share.  Everything comes ready-to-go.

## Open Source

**ARMstrap is open.** ARMstrap boards can be use both personally and commercially.  We publish our schematics and design files under an [MIT license][4], giving you the flexibility to use, change, remix and do whatever you need. We hope you will mention us in your project, but if you don’t, that’s fine too.

## Remixable

A remixable project is a project that can easily be changed and re-purposed to suit different needs.  Many projects ship the schematic but often fail to ship the CAD design program.  **ARMstrap boards ship the Eagle CAD Design Files, which work on Mac, Linux and Windows platforms.**

**All ARMstrap boards are designed to fit a two-layer PCB board.** Many PCB fabricators can crank out two-layer boards easily and in a cost effective manner, giving your project the agility it needs. There are also several online prototyping services that can ship a two-layer board in a very cost effective manner. Agility and keeping costs down are really important characteristics for remixability.

Working with a community means accommodating to different talents and needs. **All ARMstrap boards can be built by regular human beings with average soldering skills.** They should not use 0201 or 0402 sized components because they are too small to handle. They should also not use BGA components either.


[1]: http://www.keil.com/support/man/docs/ulink2/ulink2_hw_connectors.htm
[2]: http://www.mouser.com/ProductDetail/Segger-Microcontroller/J-Link-9-Pin-Cortex-M-Adapter/?qs=%2fha2pyFadugZ0p1WCusI2WIJx5gxCpe%2fsoQL3CwsvdEMANcPDBQJ%2fg%3d%3d
[3]: https://launchpad.net/gcc-arm-embedded
[4]: http://opensource.org/licenses/MIT

