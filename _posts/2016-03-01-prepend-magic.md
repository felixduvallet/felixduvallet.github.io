---
layout: post
title: File prepending magic
---

To prepend some text at the start of each file, use sed:

    sed -i '1i <pattern>' <files>

### Useful examples:

Add emacs headers for LaTeX mode:

    sed -i '1i % -*- mode:LaTeX; mode:visual-line; mode:flyspell -*-' *.tex
