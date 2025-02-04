---
layout: post
title: Unittesting ROS in python
---

Setting up unit tests for ROS python modules is a little tricky, but once it's in place you can easily automate testing of ros nodes.

Here is a very brief reference.

<!--excerpt-->

### Imports

import must look like:

    from <package>.module.module.file import Blah

The package and all modules must have an `__init__.py` file

### main code

In `__main__`, use:

    rostest.rosrun('package_name', 'test_name', TestCase)

Note this will also run with nosetests, but you can only run it directly using:

    rosrun <package> test_foo.py.

Calling `python test_foo.py` directly will fail.

### Executable flag

Flag must be *off* for test files (otherwise nosetests will ignore it).
