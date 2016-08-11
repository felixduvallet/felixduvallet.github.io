---
layout: post
title: An awesome system monitor.
---

I found a really nice system monitor called [Glances](http://nicolargo.github.io/glances/):

![screenshot](http://glances.readthedocs.io/en/latest/_images/screenshot-wide.png "Glances screenshot")

Installing is super simple:

    $ sudo pip install glances
    $ glances


You can also run this in web mode, which is useful for visualizing the system load on a remote server somewhere:

    $ glances -w

Then, just point your browser to http://@server:61208

NOTE that you need to have bottle installed: `$ sudo pip install bottle`.
