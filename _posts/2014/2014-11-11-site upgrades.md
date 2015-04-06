---
layout:   post
comments: true
title:    "Fast and Furious Upgrades"
category: Upgrades
---

We've been busy upgrading...pretty much everything.

![Fast and Furious Upgrades](/img/posts/2014/11/fast_and_furious_6.jpg){: .centered .img-responsive}

The armstrap.org site is composed of two sections: a blog section and a community section.  Both sections have been upgraded and are now insanely fast and much more scalable.

* The blog section used to be an Amazon EC2 Linux VM with 512MB of RAM hosting WordPress.  That was fine as long as traffic was low.  When traffic got high, the machine would crash due to memory constraints.  Finally, when a failed WordPress update took down the php-engine (the engine used to run WordPress), we looked at other, easier to maintain blog engines.  We settled on [jekyll][1] (hosted on [github page][2]) because it was easy to use and much more scalable.  All posts are now simple markdown text files used to generate static html pages.

* The Community section also got a major upgrade.  We went from an Amazon EC2 single-core 4GB of RAM HD-based Linux VM to a Microsoft Azure dual-core 8GB of RAM SSD-based Linux VM.  This has helped significantly improve the performance of the community site.  The software behind the community site, [Discourse][3], also got an upgrade.

We hope you enjoy the improvements.

[1]: http://jekyllrb.com
[2]: http://jekyllrb.com/docs/github-pages/
[3]: http://www.discourse.org
