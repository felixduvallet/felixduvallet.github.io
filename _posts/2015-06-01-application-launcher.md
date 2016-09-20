---
layout: post
title: Ubuntu application launcher
---

Ubuntu/Mint application launcher files live in: `/usr/share/applications`

To change the command that gets called when launching an application from the
system menu, change the 'Exec' line in the appropriate file.

For example, changing:
    jetbrains-pycharm-ce.desktop
To execute the command:
    Exec=bash -i -c "/opt/pycharm/pycharm/bin/pycharm.sh" %f
