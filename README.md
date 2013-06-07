Node-2-Node
===========

[Nei.ghbor.Net](http://Nei.ghbor.Net) Umbrella repository. Here we collect the various pieces of the Nei.ghbor.Net puzzle in one place.
for an outline of the motivations and design considerations of the project, see **[Why](http://Nei.ghbor.Net/main/why/)** and **[How](http://nei.ghbor.net/main/how/)**

You Want to Contribute?
=======================

#### Here's our [Gameplan](https://www.pivotaltracker.com/s/projects/834121)

Give us a shout and we'll add you to the [pivotal](https://www.pivotaltracker.com/s/projects/834121).

Overview
========

Node-2-Node collects various parts of the Nei.ghbor.Net schema for easy access to new users. Development of each part occurs in it's own repo.
It is our hope that this repository will eventually contain all necessary code for a new node to set up with as little friction as possible.

We divide the Nei.ghbor.Net project into 4 categories:

* Nei.ghbor.Net Ground - The Routing protocol stack (CCNx and CJDNS, both developed elsewhere but mirrored here)
* Nei.ghbor.Net Keystone - The Logic for using Nei.ghbor.Net-Ground to route content based on geographical location
* Nei.ghbor.Net Lightning - Basic Reference webserver and client API to allow application development based on Keystone
* Nei.ghbor.Net Apps - Demonstration applications powered by lightning

The dream: Someone wants to be a part of the project. They install Ground, configure Keystone, intitialise lighting, and apply some apps. Then they point their neighbors to their new website.

Getting Started:
================

Initialize Git Submodules:

```bash
# on initial clone
git submodule init
git submodule update  # this clones the repos the first time

# when the submodule sha's change
git submodule update  # this now pulls down any upstream changes
```
