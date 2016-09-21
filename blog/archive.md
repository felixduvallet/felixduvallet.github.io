---
layout: archive
title: Blog Archive
---

<!-- use 'archive' layout, which is just a copy of 'page' with
     a different name so this page doesn't appear in the sidebar. -->

## Disclaimer

I use github-page's blogging capability solely as a self-reference space for odd memos and random documentation, so that I can safely forget useful things I come across (until the next time I need them).

Nevertheless, I've decided to make these accessible, even though (as you can see) they are primarily intended for an audience of myself.

If these are helpful to you, or (more likely) if you have a better way to do something, please let me know.

## Blog Posts

{% for post in site.posts %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})
{% endfor %}
