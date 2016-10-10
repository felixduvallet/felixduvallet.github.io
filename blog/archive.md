---
layout: archive
title: Blog Archive
---

<!-- use 'archive' layout, which is just a copy of 'page' with
     a different name so this page doesn't appear in the sidebar. -->

## Disclaimer

I use github-page's blogging capability primarily as a self-reference space for odd memos and random documentation, so that I can safely forget useful things I come across (until the next time I need them).
If I happen to do something interesting and worth sharing I've been known to write that up, but it's pretty rare.

I've decided to make all my memos accessible, even though (as you can see from the lack of formatting) they are primarily intended for an audience of myself.

If these are helpful to you, or (more likely) if you have a better way to do something, please let me know.

## Blog Posts

{% for post in site.posts %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})
{% endfor %}
