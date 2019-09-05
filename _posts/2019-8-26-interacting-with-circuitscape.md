---
layout: post 
title: Interacting with Circuitscape

categories: blog
---

**Summary**: We introduce a new way of interacting with Circuitscape via a
light command line utility, deprecrating the old graphical user interface. 

![](/assets/inibuilder.gif)

Today we announce the release of INIBuilder, a command line utility for
building Circuitscape problems. This will replace and effectively deprecate
the current Circuitscape GUI project and will be the de-facto way to
specify and run Circuitscape problems. 

## Deprecating the Graphical User Interface 

Usually, users interact with Circuitscape via a graphical user interface (GUI). 
But throughout our development process, we had significant problems with them.

1. GUIs are hard to maintain. 

1. Command line UIs are much easier to maintain than GUIs 
which are time consuming to maintain and ship.  The command line utility
is much easier to maintain, and is built upon native utilities in the Julia standard
library. Additionally, the packages that the Circuitscape v4 GUI was 
written with are currently unmaintained.
2. GUIs are quite heavy. The new Circuitscape GUI was based on Electron. 
Electron works on both Windows and MacOS but it also ships with a version
of Chromium. We shouldn't need to ship an entire web browser to run Circuitscape. 
INIBuilder is much lighter, using only a simple commands and functions. 


## How does it work?

The UI is kicked off by calling the `start()` function, which brings you to
a wizard. The sequence of steps is very similar to the steps in the user
