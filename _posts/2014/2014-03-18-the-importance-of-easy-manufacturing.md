---
layout: post
title:  "The Importance of Easy Manufacturing"
---
What [experts predicted][1] has finally happened.  People are using the [BeagleBone Black][2] and [Raspberry Pi][3] for more than just prototyping.  They are using them as critical pieces to their deployed solution.

There's just one problem.  These tiny all-in-one mini computers were never designed to be deployed in an end-product.

![BeagleBone Black Assembly](/img/posts/2014/03/beaglebone-black-assembly.png){: .centered .img-responsive}

[Companies that sell][4] the BeagleBone Black are now reporting huge backlogs totaling [14,000 units][5].  It's really hard to get a hold of these boards and according to Gerald Coley, the designer of the BeagleBone Black and systems engineer at Texas Instrument (the company sponsoring the BeagleBone Black), the problem is not going away anytime soon.

Gerald [writes][6]...

> We have doubled our production over the last two months to 3,000 per week. But that is about as good as it is going to get. We still have people sucking up 100s of boards for use in products and we have not found a way to stop that. We are building them and we are shipping them as fast as we can. They just aren't getting to people that we want to have them.

The BeagleBone Black and Raspberry Pi fall into a category of electronics I call the put-everything-on-a-pcb-and-make-it-cheap type of device.  They don't need to worry about drivers because they have their own on-board operating system.  These solutions make prototyping a joy because they offer fertile soil to grow the seeds of a maker's dream.

There is just one big problem: these solutions do not scale.

These all-in-one boards seduce entrepreneurs, who find themselves at a loss when it comes time to scale their solution.  Naturally, these startups cannot reproduce any of these low cost devices and preserve their low price point.  Yes, they are open source and that's a big win.  But if you cannot scale your solution, why would any startup consider using one of these all-in-one devices?  Why would your core component be tied to another company's supply chain?

Armstrap is  different.  **We care about the ability to mass produce your solution.**  That's why the [Armstrap Eagle][7] is made using 0805-sized components on a simple 2-layer PCB.  They can easily be recreated by hand if need be.  And thanks to its open-source license and to services like [OSH Park][8] and [OSH Stencils][9] anyone can remix the board and hand-solder a new prototype.  If your Kickstarter is massively successful, then you can make the adjustments necessary to lower costd: for example eliminating the integrated JTAG debugger if its not required.

Rather than giving makers everything on a board and slapping an operating system on top, **we embrace the hardware and focus on making it easier to develop, debug and deploy your solution.**

Want to buy an Armstrap Eagle?  We [sell them on the website][7], however, they can be built by hand too.  More on that later.

[1]: http://www.digikey.com/en/articles/techzone/2013/jun/life-after-pi
[2]: http://beagleboard.org/Products/BeagleBone+Black
[3]: http://www.raspberrypi.org/
[4]: http://mx.mouser.com/new/embedded-solutions/beagleboneblack
[5]: http://mx.mouser.com/ProductDetail/CircuitCo/BB-BBLK-000/?qs=%2fha2pyFadugh6wNMONnDuAbTwbrIHVw4R%2f%252bth5Q2M%2fX2Gs60muroNw%3d%3d
[6]: https://groups.google.com/forum/#!topic/beagleboard/Z3JfUIkxOl8[101-125-false]
[7]: /eagle
[8]: https://oshpark.com/
[9]: http://www.oshstencils.com/



