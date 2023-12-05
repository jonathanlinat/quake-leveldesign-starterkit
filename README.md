<p align="center"><img src="https://camo.githubusercontent.com/55ce69ebaf4bbabe5a3e87f9f744a5fba22991fb9d185b2301567cb67e6a9193/68747470733a2f2f696d6167652e6962622e636f2f636f667974652f7175616b656c6576656c64657369676e737461727465726b69745f6c6f676f2e706e67"></p>
<h1 align="center">Quake Level Design Starter Kit</h1>

The **Quake Level Design Starter Kit**, also known as **QLDSK**, consolidates a variety of tools and resources into one comprehensive package, facilitating the quick and easy creation of Quake-based maps with just a few clicks.

---

## Weekly Release

| 🔔 Get the Latest Weekly Release |
|----------------------------------|
| [![Latest Weekly Release](https://badgen.net/github/release/jonathanlinat/quake-leveldesign-starterkit?icon=github&label=Release)](https://github.com/jonathanlinat/quake-leveldesign-starterkit/releases/latest) |

Great, you're all set! Now, [proceed to the installation](#installation).

### Automated Workflow

This project operates on an automated system, meaning the tools are compiled every week from their original source codes available on GitHub, while additional resources are securely sourced from legitimate and reputable websites.

| 🏗️ Continuous Building Status | 📦 Continuous Packing Status | 🚀 Continuous Releasing Status |
|-------------------------------|------------------------------|--------------------------------|
| [![Continuous Building](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-building.yml/badge.svg)](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-building.yml) | [![Continuous Packing](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-packing.yml/badge.svg)](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-packing.yml) | [![Continuous Releasing](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-releasing.yml/badge.svg)](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-releasing.yml) |

Two artifacts are released, offering compatibility with the following operating systems:

> ⚠️ **Important**: Only 64-bit versions are supported.

- **Microsoft Windows**
- **Linux** (specifically for Debian-based distributions)

---

## Features

The current version of **QLDSK** includes the following set of tools and extras:

### Tools

* **ericw-tools**, Eric Wasylishen [[GitHub](https://github.com/ericwa/ericw-tools)] [[Website](https://ericwa.github.io/ericw-tools)]
  - A suite of command-line utilities for building levels (maps) for games like Quake and Hexen 2, and represent an evolved branch of Tyrann's original Quake tools. The tools focus on adding advanced lighting features, some of which are borrowed from q3map2, and include bugfixes for the qbsp tool, which is used for constructing the block structure of the map.
* **Ironwail**, Andrei Drexler [[GitHub](https://github.com/andrei-drexler/ironwail)] [[Twitter](https://twitter.com/andrei_drexler)] 
  - An advanced fork of QuakeSpasm, a popular source port of the Quake engine, aimed at enhancing performance and introducing additional features. It has been optimized for high performance, incorporating modern techniques such as culling, GPU-accelerated lightmap updates, and compute shaders, allowing it to handle highly detailed Quake maps at very high framerates.
* **Quake CLI Tools**, Joshua Skelton [[GitHub](https://github.com/joshuaskelly/quake-cli-tools)] [[Website](https://joshua.itch.io/quake-tools)] [[Usage](https://www.youtube.com/watch?v=zJ0RX62VYaA)]
  - A collection of command-line utilities to facilitate the creation of content for the Quake game series. These tools can perform various tasks, including managing PAK and WAD files, such as adding and extracting files, converting BSP files to WAD files, and even creating SVG files from BSP files.
* **TrenchBroom**, Kristian Duske [[GitHub](https://github.com/TrenchBroom/TrenchBroom)] [[Website](http://kristianduske.com/trenchbroom)]
  - A free, open-source, cross-platform level editor designed explicitly for Quake-engine-based games. It is compatible with games like Quake, Quake 2, and Hexen 2 and can be run on multiple operating systems. It is recognized for its ease of use, offering simple and advanced tools that enable designers to craft complex and engaging levels without much hassle.

### Extras

* **Prototype WAD**, Aleksander Marhall [[Source](https://www.slipseer.com/index.php?resources/prototype-wad.263)]
  - A resource containing Quake textures designed for map prototyping. It features 273 prototype textures that are indexed to Quake's palette. The collection includes basic checker textures in eight base colors, three shades, and four different sizes (16x16, 32x32, 64x64, and 128x128). It also contains solid color textures, which include fullbright colors, and specialized textures.
* **TrenchBroom Quake Map Source**, Atul Varma [[Source](https://book.leveldesignbook.com/appendix/resources/quake)]
  - A collection of the original Quake 1 MAP source files, as released by John Romero in 2006. These files have been converted to a modern file format that is compatible with TrenchBroom. Additionally,  the texture references in these files have been fixed with a repackaged `quake101.wad` file.

---

## Project Structure

The organization of **QLDSK** is as follows:

```text
.
├── extras/         # Contains third-party resource files
├── game/           # Houses the game engine and associated data
├── level-editor/   # Stores the level editor's binaries
└── tools/          # Holds the tool binaries
```

---

## Installation

### Software Requirements

* A legitimate copy of Quake [[Steam](https://store.steampowered.com/app/2310)] [[Good Old Games](https://www.gog.com/game/quake_the_offering)]
* For **Microsoft Windows** users:
  - Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019 [[x64](https://aka.ms/vs/16/release/vc_redist.x64.exe)]

### Download

Get the [latest ZIP release](https://github.com/jonathanlinat/quake-leveldesign-starterkit/releases) and extract its contents into a directory, likely named `quake-leveldesign-starterkit-<date>-<os>`.

### First Setup

Find and open the `quake-leveldesign-starterkit-<date>-<os>` directory in your files explorer.

Create two new directories:

* An `id1` directory within the `game` directory.
* A `maps` directory inside the `id1` directory for saving compiled maps.
* A `working` directory at the root, which will remain empty until the `ericw-tools` compiler is utilized, and where the MAP and other related files will be hosted.

Lastly, from your original Quake game installation, copy the `pak0.pak` file into the `id1` directory. These files are necessary to test your map using `Ironwail`.

> ℹ️ **Note**: These instructions are also applicable to other expansions and modifications.

Here is what you should have at the end of the process:

```text
.
├── extras/
├── game/
│   └── id1/
│       ├── maps/
│       └── pak0.pak
├── level-editor/
├── working/
└── tools/
```

> ⚠️ **Important**: Users on Unix systems need to grant execution rights to binaries.
>
> To set execution permissions recursively from the **QLDSK** directory, execute this command in your Terminal: `find . -type f -exec sh -c 'file -b "{}" | grep -q "^ELF"' \; -exec chmod +x "{}" \;`.

---

## Getting Started

To assist you in effectively utilizing the tools included in this starter kit, consider these two informative articles for guidance:

> ℹ️ **Note**: The procedures outlined might slightly vary from the current project structure.

* **Setting up TrenchBroom in Ubuntu to create and compile Quake maps**, s3thra [[Website](https://quake.blog/trenchbroom-ubuntu-setup-tutorial.html)]
* **Configure TrenchBroom in Windows to create Quake maps**, s3thra [[Website](https://quake.blog/configure-trenchbroom-in-windows.html)]

### Basic Usage

The inspiration for this project primarily comes from the excellent series of video tutorials by [dumptruck_ds](https://twitter.com/david_spell). Be sure to explore these [informative videos](https://www.youtube.com/playlist?list=PLgDKRPte5Y0AZ_K_PZbWbgBAEt5xf74aE)!

<p align="center"><a href="https://www.youtube.com/watch?v=gONePWocbqA" align="center"><img src="https://img.youtube.com/vi/gONePWocbqA/0.jpg"></a></p>

---

## Additional Resources

* **The Level Design Book**, Robert Yang [[Website](https://book.leveldesignbook.com)]
  - This online resource compiles a wealth of information on 3D video game level design in a contemporary and accessible manner. It caters to designers across all levels of experience and various game engines.
* **Quaddicted**, Spirit [[Website](https://www.quaddicted.com)]
  - A fan site dedicated to the iconic game Quake, renowned for its comprehensive archive of Quake singleplayer maps. The site also includes installation tools, a range of archives featuring engines, tools, wads, multiplayer maps, and informative articles, catering to the needs of both Quake players and developers.
* **Slipgate Sightseer**, Michael Markie [[Website](https://www.slipseer.com)]
  - A website dedicated to the Quake modding community. It offers a variety of content related to Quake, a popular first-person shooter game known for its modding capabilities and active community support. The site features tools and resources for both players and modders of Quake.
* **Quake.blog**, s3thra [[Website](https://quake.blog)]
  - A comprehensive blog that began as a platform to document the creator's experiences with TrenchBroom, Quake map creation, and playing Quake map packs. The blog has grown to include a variety of content including tutorials, personal stories, and videos, extending beyond the realm of Quake to cover other topics as well.
* **Func_Msgboard**, John Fitzgibbons [[Website](https://www.celephais.net)]
  - A significant forum and online community focused on video game level design, particularly for games using the Quake engine. For over twenty years, it has been a central hub for both hobbyist and professional level designers to exchange ideas and engage in discussions about game development.
* **Quaketastic** [[Website](https://www.quaketastic.com)]
  - Hosts an extensive collection of reusable resources, available through a comprehensive file browser.
