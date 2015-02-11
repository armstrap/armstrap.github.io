---
layout: post
title:  "Documentation Facelift"
---

![Guy in Subway Reading](/img/posts/2013/12/jens-schott-knudsen-flickr.jpg){: .centered .img-responsive}

I think that for any open-hardware community to thrive, that community has to have insanely-great documentation.  Great documentation is not just in the form of web pages on a screen, but also PDF and ePub documentation that you can take on-the-go.  Documentation teaches others how to use your product and learning and discovery is a big part of Armstrap.

Like most engineers, I find documentation hard.  They are great to read, but difficult to write.  Why?  Because too often, documentation becomes a war of styles, tags, placement and deployment.  Like programming, documentation is riddled with rules and getting the simplest projects off the ground requires an enormous amount of effort.  This enormous effort has nothing to do with the message you are trying to convey.  Rather than helping you, they stand in your way, forcing you to learn their quirks.  Writing anything will take time because the author has to overcome these hurdles.  Luckily, two technologies exists that can alleviate much of this pain–[reStructuredText][1] and [readthedocs.org][2].

reStructuredText is a markdown language that is incredibly rich in syntax and easy to learn.  It does a fantastic job hiding those complex XML/HTML/DocBook tags, giving authors the freedom to express themselves in a plain-ol’ text editor.  Unlike those tag-based approaches to documentation, reStructuredText has no tags.  That’s right.  None.  reStructuredText uses an intelligent approach to documentation where styling and formatting is inferred based off text spacing and layout.  If you have five minutes, check out the [reStructuredText cheatsheet][3] and the [online editor][4].  I found it amazing how fast and easy it was to learn.  Try doing this with DocBooks.

But what about deployment?  Getting documentation written is one challenge but deployment can be a greater challenge.  Generating HTML, PDF, and ePub for consumers can be an equally difficult task.  That’s where Read the Docs come in.

The readthedocs.org service is amazing!  In a nutshell, they translate reStructuredText from a github repository into beautiful, clean documentation.  They automatically generate HTML, PDF and ePub front-ends that make documentation kind of fun.  It’s free and it looks fantastic, even on a mobile device.  Did I say this happens automatically?  If you have five minutes, check out their [screencast][5].

We recently revamped our [tutorials and getting started guides][6] to use reStructuredText and readthedocs.org.  In the future, we plan on getting more tutorials and guides published using these technologies.  Documentation is fun again!

[1]: http://docutils.sourceforge.net/rst.html
[2]: https://readthedocs.org/
[3]: http://docutils.sourceforge.net/docs/user/rst/quickref.html
[4]: http://rst.ninjs.org/
[5]: https://www.youtube.com/watch?feature=player_embedded&v=oJsUvBQyHBs
[6]: http://docs.armstrap.org/
