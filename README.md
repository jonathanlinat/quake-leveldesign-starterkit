# Quake Level Design Starter Kit

![](https://image.ibb.co/cofyte/quakeleveldesignstarterkit_logo.png)

This **Starter Kit** is mainly based on files / directory structure and set of tools recommended by [dumptruck_ds](https://twitter.com/david_spell).

_Note: Only for Microsoft Windows (x86-64) users._

## Features

It includes:

* Quakespasm Spiked 0.93.2ish (2021-July-08), Spoike [[Link](https://triptohell.info/moodles/qss/)]
* TrenchBroom 2021.1, Kristian Duske [[Link](http://kristianduske.com/trenchbroom)]
* ericw-tools 0.18.1, Eric Wasylishen [[Link](https://ericwa.github.io/ericw-tools)]
* ne_q1spCompilingGui 1.0.3, C. Jones [[Link](https://shoresofnis.wordpress.com/utilities/ne_q1spcompilinggui)]

Extras:

* Quake Tools 1.2.1, Joshua Skelton [[Link](https://joshua.itch.io/quake-tools)] [[Usage](https://www.youtube.com/watch?v=zJ0RX62VYaA)]
* TexMex 3.4, Mike Jackman [[Link](https://quakewiki.org/wiki/TexMex)]
* Map2Curve 0.7, ToTac [[Link](http://gibshooter.com/map2curve)]
* Original Quake maps, John Romero [[Link](https://rome.ro/news/2016/2/14/quake-map-sources-released)]
* Original Quake textures [[Link](https://www.quaddicted.com)]
* Prototype WAD textures 1.3, Aleksander "Khreathor" Marhall [[Link](http://khreathor.xyz/site/prototype)]

## Prerequisites

You need:

* Microsoft Windows: Vista, 7, 8, 10
* A legal copy of Quake [[Steam](https://store.steampowered.com/app/2310)] [[Good Old Games](https://www.gog.com/game/quake_the_offering)]
* Git [[Link](https://git-scm.com/)]
* Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019 [[x86](https://aka.ms/vs/16/release/vc_redist.x86.exe))]

## Installation

### Download

You have two options:

* Download the [latest available ZIP release](https://github.com/jonathanlinat/quake-leveldesign-starterkit/releases) and extract its content into a directory called `quake-leveldesign-starterkit`.
* Open a Terminal session and clone this Git repository:

```bash
cd <path/to/desired/directory/>
git clone https://github.com/jonathanlinat/quake-leveldesign-starterkit.git
cd quake-leveldesign-starterkit/
```

### Configuration

Locate and open `quake-leveldesign-starterkit` directory in Windows Explorer.

Create three new directories:

* The first one called `working`, located at the root directory. It'll remain empty until `ne_q1spCompilingGui` tool is used.
* The second one called `id1`, also located at the root directory.
* And the last one called `maps` into the `id1` directory. This is the directory used to save the compiled maps.

Last but not least, copy and paste into `id1` directory the original `pak0.pak` and `pak1.pak` files from your Quake game copy location. These are required in order to be able to test your map using `Quakespasm`.

## Usage and Quickstart

[![Video](http://img.youtube.com/vi/gONePWocbqA/0.jpg)](http://www.youtube.com/watch?v=gONePWocbqA)

This video tutorial is part of an awesome series created by [dumptruck_ds](https://twitter.com/david_spell). Please, [check it out](https://www.youtube.com/playlist?list=PLgDKRPte5Y0AZ_K_PZbWbgBAEt5xf74aE)!

## Credits

[Image](https://i.imgur.com/p0E4SuR.png) used to create the Starter Kit illustration.
