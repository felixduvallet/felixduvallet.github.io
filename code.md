---
layout: page
title: Code
---

Getting robots to solve big complex problems reliably requires a lot of code.
I am an active developer and have contributed both to personal projects and open-source projects.

You can find some of my useful contributions below.
For the non-useful ones, see my [github](https://www.github.com/felixduvallet) page.

#### Travis-CI for ROS

![alt-text][ros-travis]

I wrote a travis script for running continuous integration on any ROS package.
The end result is that each time you commit something on github, Travis can install ROS on a brand new virtual machine, clone your package, resolve all dependencies, build it (using catkin_make) and test it.
This work is now used by many other researchers world-wide to produce better code running on robots.

[https://github.com/felixduvallet/ros-travis-integration](https://github.com/felixduvallet/ros-travis-integration)


[ros-travis]: /assets/projects/ros-travis.png

#### Allegro Hand ROS bindings

I took over the maintenance of SimLabs's Allegro Hand bindings.
I cleaned up the package so that it could work with a modern version of ROS,
re-organized the package to bring it in line with best practices,
and made numerous other improvements.
As far as I know, this is now the most widely used ROS interface for the Allegro hand.

You can see my (unofficial) fork here:
[https://github.com/felixduvallet/allegro-hand-ros](https://github.com/felixduvallet/allegro-hand-ros)

#### Grasp synergy

I wrote a very simple package that provides convenience wrappers around the concept of a grasp synergy (low-dimensional representations of hand grasps).
[http://wiki.ros.org/grasp_synergy](http://wiki.ros.org/grasp_synergy)

##### results-filecache

I wrote a cool decorator that can "magically" determine if a function should be called (to do work) or if its results can be loaded from file (if the work has already been done).
Essentially, this is ccache for scientific processing pipelines.

This is most useful in situations where you usually do some form of pre-processing to data after loading it from files into your own structure, *then* actually analyze the data.
This can save considerable time by short-cutting the pre-processing step (which doesn't change) during development of the analysis code.

[https://github.com/felixduvallet/results-filecache](https://github.com/felixduvallet/results-filecache)

##### Other contributions

I have made very minor (sometimes trivial) contributions to many more ROS packages, which I list here for my own reference:

  * [audio_common](https://github.com/ros-drivers/audio_common)
  * [ros_buildfarm](https://github.com/ros-infrastructure/ros_buildfarm)
  * [gazebo_ros_demos](https://github.com/ros-simulation/gazebo_ros_demosros)
  * [mocap_optitrack](https://github.com/ros-drivers/mocap_optitrack)
  * [pocketsphinx](https://github.com/felixduvallet/pocketsphinx)
  * [rospy](https://github.com/ros/ros_comm/)
  * [rqt_ez_publisher](https://github.com/OTL/rqt_ez_publisher)
