---
layout: page
title: Projects
---

On this page you can find brief descriptions of various research projects I've worked on.
I also have links to various pieces of code I've written.

For more detailed information, please go see my [publications](/publications) or [github](https://www.github.com/felixduvallet) pages.

## Research

#### Human-Robot Handovers
We developed a human-inspired controller that could perform fast and fluent handovers (bi-directionally) between a human and robot team.

#### Understanding Natural Language Directions
We addressed the problem of a robot following directions through a completely unknown environment (i.e. without any prior map) and developed an approached based on imitation learning.

#### Generating Maps from Language

Extending the work on following direction, we investigated how robots could use **language as a sensor**, whereby the robot could extend the partial map it has (built using its sensors) with information that was contained in the direction.

#### Imitation Learning for Multi-Robot Coordination

We looked at how a team of robots could learn to allocate tasks using expert demonstrations, by learning the task allocation utility function.

## Code

Like it or not, robots run on code.
Getting code that runs on robots to a level that enables big complex projects to work reliably is both a skill and an art that I've been honing for many years.
I am an active developer and have contributed both to personal projects and open-source projects.

#### Travis-CI for ROS

I wrote a travis script for running continuous integration on any ROS package.
The end result is that each time you commit something on github, Travis can install ROS on a brand new virtual machine, clone your package, resolve all dependencies, build it (using catkin_make) and test it.
This work is now used by many other researchers world-wide to produce better code running on robots.

[https://github.com/felixduvallet/ros-travis-integration](https://github.com/felixduvallet/ros-travis-integration)

#### Allegro Hand ROS bindings

I took over the maintenance of SimLabs's Allegro Hand bindings.
I cleaned up the package so that it could work with a modern version of ROS,
re-organized it to bring it in line with best practices, and made numerous other improvements.

You can see my (unofficial) fork here:
[https://github.com/felixduvallet/allegro-hand-ros](https://github.com/felixduvallet/allegro-hand-ros)

#### Grasp synergy

I wrote a very simple package that provides convenience wrappers around the concept of a grasp synergy (low-dimensional representations of hand grasps).
[http://wiki.ros.org/grasp_synergy](http://wiki.ros.org/grasp_synergy)

##### results-filecache

I wrote a cool decorator that can "magically" determine if a function should be called (to do work) or if its results can be loaded from file (if the work has already been done).
Essentially, this is ccache for scientific processing pipelines.
This is most useful in situations where you usually do some form of pre-processing to data after loading it from files into your own structure, then actually analyze the data.
This can save considerable time by short-cutting the pre-processing step (which doesn't change) during future updates to the analysis code.

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

