# Homebrodot PSP

This is a fork of [Homebrodot](https://github.com/Homebrodot/Godot?tab=readme-ov-file), mainly the branch main/2.1 a port of Godot 2.1 to the PSP. It contains the changes I made to get it building and running reliably on my setup. For the full step-by-step write-up of how I got it working, see the [wiki](docs/WIKI.md).

## My setup

- **Console:** PSP 1000 with custom firmware (M33)
- **Emulator:** PPSSPP 1.20.4
- **Host OS:** Linux Mint 22.3 (Zena)
- **Toolchain:** pspdev (psp-gcc (GCC) 15.2.0) 

## Changes from the original

The main change is that I compile the `EBOOT.PBP` with `-Os` to get a smaller build, since the PSP 1000 only has 32 MB of RAM. 

There are also other fixes and tweaks, and most of the details are in the [wiki](docs/WIKI.md).

## Tutorial

A more comprehensive step-by-step tutorial covers how to build the runtime, the steps I took to make a game with it, and the tools I used along the way.

You can find it here: [wiki](docs/WIKI.md).



# Original README bellow

[![GODOT](/logo.png)](https://godotengine.org)

## Godot Engine

Homepage: https://godotengine.org

#### 2D and 3D cross-platform game engine

Godot Engine is a feature-packed, cross-platform game engine to create 2D and
3D games from a unified interface. It provides a comprehensive set of common
tools, so that users can focus on making games without having to reinvent the
wheel. Games can be exported in one click to a number of platforms, including
the major desktop platforms (Linux, Mac OSX, Windows) as well as mobile
(Android, iOS) and web-based (HTML5) platforms.

#### Free, open source and community-driven

Godot is completely free and open source under the very permissive MIT license.
No strings attached, no royalties, nothing. The users' games are theirs, down
to the last line of engine code. Godot's development is fully independent and
community-driven, empowering users to help shape their engine to match their
expectations. It is supported by the Software Freedom Conservancy
not-for-profit.

Before being open sourced in February 2014, Godot had been developed by Juan
Linietsky and Ariel Manzur (both still maintaining the project) for several
years as an in-house engine, used to publish several work-for-hire titles.

### Getting the engine

#### Binary downloads

Official binaries for the Godot editor and the export templates can be found
[on the homepage](https://godotengine.org/download).

#### Compiling from source

[See the official docs](http://docs.godotengine.org/en/latest/development/compiling/)
for compilation instructions for every supported platform.

### Community

Godot is not only an engine but an ever-growing community of users and engine
developers. The main community channels are listed [on the homepage](https://godotengine.org/community).

To get in touch with the developers, the best way is to join the
[#godotengine IRC channel](https://webchat.freenode.net/?channels=godotengine)
on Freenode.

### Documentation and demos

The official documentation is hosted on [ReadTheDocs](http://docs.godotengine.org).
It is maintained by the Godot community in its own [GitHub repository](https://github.com/godotengine/godot-docs).

The [class reference](http://docs.godotengine.org/en/latest/classes/)
is also accessible from within the engine.

The official demos are maintained in their own [GitHub repository](https://github.com/godotengine/godot-demo-projects)
as well.

There are also a number of other learning resources provided by the community,
such as text and video tutorials, demos, etc. Consult the [community channels](https://godotengine.org/community)
for more info.

[![Build Status](https://travis-ci.org/godotengine/godot.svg?branch=master)](https://travis-ci.org/godotengine/godot)
[![Code Triagers Badge](https://www.codetriage.com/godotengine/godot/badges/users.svg)](https://www.codetriage.com/godotengine/godot)
