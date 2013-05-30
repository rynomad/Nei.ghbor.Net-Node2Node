Nei.ghbor.Net Ground
====================

Ground is the fundamental network for the Nei.ghbor.Net project. A Ground Node consists of two parts:

* A CJDNS daemon - provides encrypted routing over local mesh networks and tunneling over the existing IP infrastructure.
* A CCNx daemon - provides content-based routing and caching for efficient distrobution of data.

To install this protocol stack, you would be well served to be running Linux or OSX

for CJDNS installation instructions, see that projects Readme

for CCNx, see http://blog.rungeek.com/post/1711470902/project-ccnx-how-to (ubuntu)

We are working on brew scripts for MacOS and apt repos for ubuntu to ease this process.

Once your Ground stack is up and running, you'll want to find some Neighbors to connect with... see Nei.ghbor.Net-Keystone


Install
=====

Nei.ghbor.Net Ground has a few dependencies to install:

#### On OSX (Brew)
- Use this [Gist](https://gist.github.com/dcunited001/5626815) to Install CCNx & CJDNS
- Please report any problems you have with this gist.  It still needs tests.
- Or compile CCNx & CJDNS from source

#### On Debian/Ubuntu
- Build CCNx/CJDNS from source
- TODO: build instructions

#### On RedHat/Fedora
- Build CCNx/CJDNS from source
- TODO: build instructions

#### On Debian Wheezy (Raspbian)
- Build CCNx/CJDNS from source
- While you wait, ask a friend about cross-compilers.
- TODO: build instructions

#### Source Code
- [CCNx 0.7.2 Tarball](http://www.ccnx.org/releases/ccnx-0.7.2.tar.gz) - 5/20/13 - [SHA1](http://www.ccnx.org/releases/ccnx-0.7.2.tar.gz.SHA1)

Config
=====
