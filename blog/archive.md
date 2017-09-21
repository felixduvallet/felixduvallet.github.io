---
layout: archive
title: Blog Archive
---

<!-- use 'archive' layout, which is just a copy of 'page' with
     a different name so this page doesn't appear in the sidebar. -->

## Disclaimer

I use this blog primarily as a self-reference space for useful bits of
information I find, so that I can safely forget them until the next time I need
them.  If I happen to do something interesting and worth sharing I've been known
to write that up, but it's pretty rare.

As you can tell from the bare bones notes, the intended audience is myself.

However, if these are helpful to you or (more likely) if you have a better way
to do something, please let me know.

## Blog Posts

{% for post in site.posts %}
  * {{ post.date | date_to_string }} &raquo; [ {{ post.title }} ]({{ post.url }})
{% endfor %}
