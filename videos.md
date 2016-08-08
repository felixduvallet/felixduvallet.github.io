---
layout: page
title: Videos
---


### Bidirectional Human-Robot Handovers

<iframe width="560" height="315" src="https://www.youtube.com/embed/Ac4kgipC7A0" frameborder="0" allowfullscreen></iframe>

### Following Directions in Unknown Environments

During my thesis I studied robots following natural language directions in
unknown unstructured environments.
These two videos show [CoBot](http://www.cs.cmu.edu/~coral/projects/cobot/)
following natural language directions through an unknown environment.
For more details, see our [ICRA 2013 paper](/publications).

<iframe width="560" height="315" src="https://www.youtube.com/embed/BVZjtpVtEJE" frameborder="0" allowfullscreen></iframe>

Here, the policy initially makes a mistake (going straight instead of turning
left), but the policy recovers; after the robot reaches the end of the hallway
it backtracks to the correct turn and continues with the rest of the direction.

<iframe width="560" height="315" src="https://www.youtube.com/embed/0WpP41FtM7o" frameborder="0" allowfullscreen></iframe>

### Inferring Maps from Natural Language

Working with roboticists at MIT, we developed an approach to extend the robot's
sensor range by using the information contained in the natural language
instruction.

Here, the wheelchair in the video below is instructed to "*go to the cone
that is behind the trashcan.*"
Our approach using an inferred map distribution correctly models the ambiguity
in the language (there are two trashcans in the environment), and the belief
space policy is able to correctly follow the direction even though the robot
initially goes behind the incorrect trashcan.


<iframe width="560" height="315" src="https://www.youtube.com/embed/xvcEjEI4YqA" frameborder="0" allowfullscreen></iframe>

Here the wheelchair follows the command "*go past the kitchen down the hallway
and take a right*" starting with a completely unknown map.
Once the robot senses it is in a hallway, it uses the implicit information
contained in the direction to update its distribution of possible locations for
the kitchen.
The belief space policy uses this information to take a sequence of actions
towards the destination.
For more details, see our [ICRA 2015 paper](/publications).

<iframe width="560" height="315" src="https://www.youtube.com/embed/jKV91Xqy9IA" frameborder="0" allowfullscreen></iframe>
