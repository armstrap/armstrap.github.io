---
layout:   post
comments: true
title:    "pyVirtualBench - Controlling Five Instruments from a Single Python Application"
---

![Techshop VirtualBench](/img/posts/2015/07/ni-virtualbench-python.jpg){: .centered .img-responsive}

Ever wanted to control five instruments from a single python script?  pyVirtualBench is a python library that gives to raw access to some pretty powerful engineering tools, all in a single application.

If you’ve walked into a [TechShop](http://www.techshop.ws), you’ve noticed that their electronics labs are outfitted with an interesting instrument at every station.  That instrument is National Instrument’s [VirtualBench](http://www.ni.com/virtualbench/) and it takes a radically different approach to instrumentation.  Rather than buying separate instruments (like a power supply, dmm, scope, function generator, DIO logic analyser), VirtualBench combines these instruments into a single package.  Five instruments in one convenient package.  That’s not bad.

![Techshop VirtualBench](/img/posts/2015/07/techshop-virtualbench.jpg "Image courtesy of sfgate.com"){: .centered .img-responsive}

There’s already enough [marketing material](http://www.ni.com/virtualbench/what-is) on the web so I’m not going to go into the specs of the machine.  What I’ll be talking about is the advantage of combining these instruments to get work done that was previously not possible had these instruments been separate boxes.

One of the things that has bugged me for a long time about traditional instruments is the idea that no matter the instrument, they encourage me to do things I don’t want to do.  For example, if I needed to do a series of tests on several boards, I don’t want to constantly be fiddling with my instrument’s configuration.  And when actually testing my board, I don’t want to constantly look at my display (which can sometimes be several feet away).  I want to keep my eyes on the work and my hands on my probes.

Thanks to National Instruments releasing a c-api to their driver, [I wrote a Python wrapper](https://github.com/armstrap/armstrap-pyvirtualbench/tree/master/lib) that allows me to easily interface with the VirtualBench instrument.

For this demo, I’m going to be using a simple 3-switch USB foot pedal I purchased on Amazon for about 55 US dollars.  Cheaper foot pedals exist, but I really liked the quality of this particular unit.  I’ll only be using one of the three switches but I can easily see myself using all three switches to do other things, like perhaps triggering or starting a particular measurement.

![Infinity USB Digital Foot Control](/img/posts/2015/07/usb-foot-pedal.jpg){: .centered .img-responsive}

I’ll also be using Google’s Text-to-Speech API to output my measurement to my computer’s speaker.

In my [application](https://github.com/armstrap/armstrap-pyvirtualbench/blob/master/examples/hands_free_dmm.py), I want to do three different kinds of tests: a voltage test, a resistance test and a continuity test.  I’m using the foot pedal to cycle through the various instruments.  My ears will be listening for each measurement result, allowing my eyes can stay on my work and my hands can stay on my probes.

And because my application is written in python, changes are as simple as opening and editing my script in a regular text editor, making customizations and tweaks relatively easy.

<iframe width="480" height="270" src="http://www.youtube.com/embed/1NOQRLI39es" frameborder="0" allowfullscreen></iframe>

I’m really excited about VirtualBench and I’m excited to see where this instrument will go.  Got a VirtualBench and want to try it out?  I’ve released the Python wrapper in our [GitHub repository](https://github.com/armstrap/armstrap-pyvirtualbench).  I’m excited to see what you guys can come up with.  Drop me a line if you do something cool.

