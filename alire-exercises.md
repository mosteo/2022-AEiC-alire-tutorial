---
author:
- Alejandro R. Mosteo
title: The Alire Package Manager - Exercises
institute: Professor with Centro Universitario de la Defensa, Zaragoza, Spain
twitter: mosteobotic
github: mosteo
fontsize: 15pt  # Works only for HTML export
theme: metropolis
# logo: images/cudsmallmargin # Doesn't give the margin we want, in template instead
date: Jun 14th, 2022
navigation: empty
aspectratio: 169
...

## Getting started

Visit the following repository to get the materials:

- [https://github.com/mosteo/2022-AEiC-alire-tutorial](https://github.com/mosteo/2022-AEiC-alire-tutorial)

# Installation

## Installation

 - From binaries
    - https://github.com/alire-project/alire/releases
       - Scroll down to **Assets** section and expand
    - Grab latest stable release (1.2) for your platform
       - For Windows, the installer is recommended
    - **Ubuntu** recommended for minimal friction

## Installation from sources

Useful to experiment with the latest features in the master branch

 1. `git clone --recurse-submodules https://github.com/alire-project/alire.git`
 1. `cd alire`
 1. On macOS only:
    - `export OS=macOS`
 1. `gprbuild -j0 -P alr_env`
 1. Executable generated at `bin/alr`
 1. Run e.g. `alr version`

## `alr version` output

```
$ alr version
APPLICATION
alr version:               1.2.0
libalire version:          1.2.0
compilation date:          2022-06-03 17:32:24
compiler version:          Community 2021 (20210519-103)

CONFIGURATION
config folder:             /home/jano/.config/alire
...
```

# Testing the (ecosystem) waters

## Retrieve and run a release

## Look up by name

## Look up by tag/other



# Starting crates

## Starting from scratch

## Starting from preexisting code



# Working with dependencies

## Adding a dependency via `alr`

## Changes caused by adding a dependency

## Adding a dependency manually



# Publishing

## Publishing a git commit

## Publishing a tarball