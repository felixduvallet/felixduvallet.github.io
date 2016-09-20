---
layout: post
title: Animating images
---

Create an animation (movie) from a sequence of images:

    ffmpeg -f image2 -r 1 -i filename-%04d.png -s WxH -f mpeg -r 24 foo.mpg

- replace WxH with width and height (ex: 800x600)
- The first -r1 makes the video 1 fps (input), so you can speed up/down as necessary.
- mpeg format seems to work okay with powerpoint.
