<a href="#">
    <img width="192px" height="192px" src="doc/icon.png" align="right" />
</a>

# Serial Studio

[![Build Status](https://github.com/Serial-Studio/Serial-Studio/workflows/Build/badge.svg)](https://github.com/Serial-Studio/Serial-Studio/actions/)
[![Github All Releases](https://img.shields.io/github/downloads/Serial-Studio/Serial-Studio/total.svg)](https://github.com/Serial-Studio/Serial-Studio/releases/)

Serial Studio is a multi-platform, multi-purpose serial data visualization program. The goal of this project is to allow embedded developers & makers to easily visualize, present & analyze the data generated by their projects and devices, without the need of writing specialized computer software for each project.

The need for this project arose during the development of the Ground Station Software for several CanSat-based competitions in which I participate. It's simply not sustainable to develop and maintain different GSS programs for each competition & project. The smart solution is to have one common Ground Station software and let each CanSat define how the data is presented to the end user by using an extensible communication protocol.

Furthermore, this approach can be extended to almost any type of project that involves some kind of data acquisition & measurement. If you want a more in-depth explanation of why this project exists, and what its all about, check [this blog post](https://www.alex-spataru.com/blog/introducing-serial-studio).

**NOTE:** Information regarding the communication protocol is provided in the [wiki](https://github.com/Serial-Studio/Serial-Studio/wiki/Communication-Protocol).

*Read this in other languages*: [Español](README_ES.md)

![Software usage](doc/app-usage.gif)

## Build instructions

#### Requirements

The only requirement to compile the application is to have [Qt](http://www.qt.io/download-open-source/) installed in your system. The desktop application will compile with Qt 5.15 or greater.

#### Cloning

This repository makes use of [`git submodule`](https://git-scm.com/book/en/v2/Git-Tools-Submodules). In order to clone it, execute these commands on your Terminal:

	git clone https://github.com/Serial-Studio/Serial-Studio
	cd Serial-Studio
	git submodule init
	git submodule update
	
Alternatively, just run:

	git clone --recursive https://github.com/Serial-Studio/Serial-Studio
    
#### Compiling the application

Once you have Qt installed, open *Serial-Studio.pro* in Qt Creator and click the "Run" button.

Alternatively, you can also use the following commands:

	qmake
	make -j4

## Licence

This project is released under the MIT license, for more information, check the [LICENSE](LICENSE.md) file.



