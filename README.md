# Quake Level Design Starter Kit

![](https://image.ibb.co/cofyte/quakeleveldesignstarterkit_logo.png)

This **Starter Kit** is mainly based on files / directory structure and set of tools recommended by [dumptruck_ds](https://twitter.com/david_spell).

_Note: Only for Microsoft Windows users._

## Features

It includes:

* Quakespasm 0.93.1, Fitzgibbons & Journeymen [[Link](http://www.quakespasm.sourceforge.net)]
* TrenchBroom 2019.6, Kristian Duske [[Link](http://kristianduske.com/trenchbroom)]
* ericw-tools 0.18.1, Eric Wasylishen [[Link](https://ericwa.github.io/ericw-tools)]
* ne_q1spCompilingGui 1.0.3, C. Jones [[Link](https://shoresofnis.wordpress.com/utilities/ne_q1spcompilinggui)]

Extras:

* Quake Tools 1.2.1, Joshua Skelton [[Link](https://joshua.itch.io/quake-tools)] [[Usage](https://www.youtube.com/watch?v=zJ0RX62VYaA)]
* TexMex 3.4, Mike Jackman [[Link](https://quakewiki.org/wiki/TexMex)]
* Map2Curve 0.7, ToTac [[Link](http://gibshooter.com/map2curve)]
* Original Quake maps, John Romero [[Link](https://rome.ro/news/2016/2/14/quake-map-sources-released)]
* Original Quake textures [[Link](https://www.quaddicted.com)]
* Prototype WAD textures 1.2, Aleksander "Khreathor" Marhall [[Link](http://khreathor.xyz/site/prototype)]

## Prerequisites

You need:

* Git [[Link](https://git-scm.com/)]
* A legal copy of Quake [[Steam](https://store.steampowered.com/app/2310)] [[Good Old Games](https://www.gog.com/game/quake_the_offering)]
* Microsoft Visual C++ Redistributable for Visual Studio 2017 [[x86](https://download.microsoft.com/download/e/6/6/e66c5871-7afe-4640-a454-786eabe8aae8/vc_redist.x86.exe)] [[x64](https://download.microsoft.com/download/7/2/5/72572684-052f-4aa9-9170-9d40813a87be/vc_redist.x64.exe)]

## Installation

### Download

You have two options:

* Download the [latest available ZIP release](https://github.com/jonathanlinat/quake-leveldesign-starterkit/releases) and extract its content into a folder called `quake-leveldesign-starterkit`.
* Open a Terminal session and clone this Git repository.

### Configuration

Locate and open `quake-leveldesign-starterkit` folder in Windows Explorer.

Create three new folders:

* The first one called `working`, located at the root directory. It'll remain empty until `ne_q1spCompilingGui` tool is used.
* The second one called `id1`, also located at the root directory.
* And the last one called `maps` into the `id1` folder. This is the folder used to save the compiled maps.

Last but not least, copy and paste into `id1` folder the original `pak0.pak` and `pak1.pak` files from your Quake game copy location. These are required in order to be able to test your map using `Quakespasm`.

## Usage and Quickstart

[![Video](http://img.youtube.com/vi/gONePWocbqA/0.jpg)](http://www.youtube.com/watch?v=gONePWocbqA)

This video tutorial is part of an awesome series created by [dumptruck_ds](https://twitter.com/david_spell). Please, [check it out](https://www.youtube.com/playlist?list=PLgDKRPte5Y0AZ_K_PZbWbgBAEt5xf74aE)!

## Credits

[Image](https://i.imgur.com/p0E4SuR.png) used to create the Starter Kit illustration.
