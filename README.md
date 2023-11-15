# Quake Level Design Starter Kit

![](https://image.ibb.co/cofyte/quakeleveldesignstarterkit_logo.png)

This **Starter Kit** primarily consists of files, directory structure, and tools recommended by [dumptruck_ds](https://twitter.com/david_spell).

> ⚠️ **Important Note**: For Microsoft Windows (x86-64) users only.

## Features

Main Tools:

* **TrenchBroom** `2023.1`, Kristian Duske [[Link](http://kristianduske.com/trenchbroom)] [[GitHub](https://github.com/TrenchBroom/TrenchBroom)]
* **Quakespasm** `0.96.1`, Eric, Ozkan & Steven [[Link](https://quakespasm.sourceforge.net)] [[SourceForge](https://sourceforge.net/projects/quakespasm/)]
* **ericw-tools** `0.18.1`, Eric Wasylishen [[Link](https://ericwa.github.io/ericw-tools)] [[GitHub](https://github.com/ericwa/ericw-tools)]
* **ne_q1spCompilingGui** `1.0.3`, C. Jones [[Link](https://shoresofnis.wordpress.com/utilities/ne_q1spcompilinggui)] [[GitHub](https://github.com/necros0/ne_q1CompilingGui)]

Extras:

* **Quake Tools** `1.2.1`, Joshua Skelton [[Link](https://joshua.itch.io/quake-tools)] [[GitHub](https://github.com/joshuaskelly/quake-cli-tools)] [[Usage](https://www.youtube.com/watch?v=zJ0RX62VYaA)]
* **TexMex** `3.4`, Mike Jackman [[Link](https://quakewiki.org/wiki/TexMex)]
* **Map2Curve** `0.7`, ToTac [[Link](http://gibshooter.com/map2curve)] [[GitHub](https://github.com/Gibshooter/Map2Curve)]
* **Prototype WAD textures** `1.3`, Aleksander Marhall [[Link](https://www.slipseer.com/index.php?resources/prototype-wad.263)]
* **Original Quake maps**, John Romero [[Link](https://rome.ro/news/2016/2/14/quake-map-sources-released)]
* **Original Quake textures** [[Link](https://www.quaddicted.com)]

## Project Structure

```text
.
├── quakespasm               # Quakespasm executable files
├── source                   # Original Quake map files
├── tools
│   ├── ericw-tools          # ericw-tools executable files
│   ├── Map2Curve_v0.7       # Map2Curve executable files
│   ├── ne_q1spCompilingGui  # ne_q1spCompilingGui executable files
│   ├── quake-tools          # Quake Tools executable files
│   └── texmex               # TexMex executable files
├── trenchbroom              # TrenchBroom executable files
└── wads                     # Original Quake texture files + Prototype WAD texture files
```

## Software Requirements

Necessary:

* Microsoft Windows: Vista, 7, 8, 10
* A legitimate copy of Quake [[Steam](https://store.steampowered.com/app/2310)] [[Good Old Games](https://www.gog.com/game/quake_the_offering)]
* Git [[Link](https://git-scm.com/)]
* Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019 [[x86](https://aka.ms/vs/16/release/vc_redist.x86.exe)] [[x64](https://aka.ms/vs/16/release/vc_redist.x64.exe)]

## Installation

### Download

Choose one of the following:

* Download the [latest ZIP release](https://github.com/jonathanlinat/quake-leveldesign-starterkit/releases) and extract its content to a directory named `quake-leveldesign-starterkit`.
* Open a Terminal session and clone this Git repository:

```bash
cd <path/to/desired/directory/>
```

```bash
git clone https://github.com/jonathanlinat/quake-leveldesign-starterkit.git
```

```bash
cd quake-leveldesign-starterkit/
```

### Configuration

Find and open the `quake-leveldesign-starterkit` directory in Windows Explorer.

Create three new directories:

* A `working` directory at the root, which will remain empty until the `ne_q1spCompilingGui` tool is utilized.
* An `id1` directory within the `quakespasm-spiked` directory.
* A `maps` directory inside the `id1` directory for saving compiled maps.

Lastly, copy and paste the original `pak0.pak` and `pak1.pak` files from your Quake game copy location into the `id1` directory. These files are necessary to test your map using `Quakespasm`.

## Getting Started

[![Video](http://img.youtube.com/vi/gONePWocbqA/0.jpg)](http://www.youtube.com/watch?v=gONePWocbqA)

This video tutorial is part of a fantastic series by [dumptruck_ds](https://twitter.com/david_spell). Don't forget to [check it out](https://www.youtube.com/playlist?list=PLgDKRPte5Y0AZ_K_PZbWbgBAEt5xf74aE)!

## Acknowledgments

The [image](https://i.imgur.com/p0E4SuR.png) utilized to create the Starter Kit illustration.
