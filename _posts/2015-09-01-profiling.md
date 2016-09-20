---
layout: post
title: Profiling your code in C++ or Python
---

(Note: this posts exists more to help me jog my own memory than to serve as a truly useful reference.)

#### C/C++

Use valgrind to profile, and kcachegrind to visualize.

    valgrind --tool=callgrind ./program
    kcachegrind callgrind.out.NNNN

#### python

Use cProfile to profile, and snake to visualize.

    python -m cProfile -o out.prof program.py
    runsnake out.prof
