---
layout: post
title: Using the IEEEtran class for Robotics conferences
---

IEEE-RAS provides some LaTeX template files for conferences but:

 - The IEEEtran.cls file has somehow been renamed ieeeconf.cls, which
   clashes with another package actually named IEEEconf and is
   confusing (IEEEconf is a separate class used for IEEE Computer
   Society manuscripts).
 - The version provided is 1.6b, instead of 1.7
 - The sample document uses deprecated commands (\overrideIEEEmargins)

This post is about getting your document to work with the current release of IEEEtran.

<!--excerpt-->

-----------------------------------------------------------

Disclaimer: These instructions are primarily for personal reference,
so that I can safely forget about this until the next time I need
them.

These worked for me, they are *a* solution but probably not the
best/optimal one.  If you've got a better way, I'd love to hear it to
update this guide.

-----------------------------------------------------------

Add these to your preamble:

{% highlight latex %}
\newcommand{\CLASSINPUTtoptextmargin}{19mm}
\newcommand{\CLASSINPUTbottomtextmargin}{18mm}
\newcommand{\CLASSINPUTinnersidemargin}{19mm}
\newcommand{\CLASSINPUToutersidemargin}{19mm}
{% endhighlight %}

These commands should be before your \documentclass command.  They set the margins manually to those specified by RAS:
[http://ras.papercept.net/conferences/support/page.php](http://ras.papercept.net/conferences/support/page.php)

Note the top text margin is the one for all but the first page.  The
first page top margin will be set later.

Then, specify the document class:

{% highlight latex %}
\documentclass[letterpaper, conference]{IEEEtran}
{% endhighlight %}

The document class should be IEEEtran, which provides support for
conferences, journals, and tech reports.  IEEEconf is actually only
used for IEEE Computer Society manuscripts.

{% highlight latex %}
\title{\vspace{6mm}Paper Title}
{% endhighlight %}

Because the title page wants an extra 6mm, we must manually introduce
a vertical offset in the title.

You should run your paper through the PDF test to check your paper for compliance: [https://ras.papercept.net/conferences/scripts/pdftest.pl](https://ras.papercept.net/conferences/scripts/pdftest.pl). The full test will check margins.
