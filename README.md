<p align="center"><img src="https://github.com/jonathanlinat/quake-leveldesign-starterkit/assets/14064112/03402bb0-65fe-4b86-a95d-3b92aeb044b7"></p>
<h1 align="center">Quake Level Design Starter Kit</h1>

The **Quake Level Design Starter Kit**, also known as **QLDSK**, consolidates various tools and resources into one comprehensive package, facilitating the quick and easy creation of Quake-based maps with just a few clicks.

---

## Weekly Release

| 🔔 Get the Latest Weekly Release |
| -------------------------------- |
| [![Get the Latest Weekly Release](https://badgen.net/github/release/jonathanlinat/quake-leveldesign-starterkit?icon=github&label=Release)](https://github.com/jonathanlinat/quake-leveldesign-starterkit/releases/latest) |

Great, you're all set! Now, [proceed to configure the kit](#first-setup).

### Automated Workflow

This project operates on an automated system, meaning the tools are compiled weekly from their source codes available on GitHub. In contrast, additional resources are securely sourced from legitimate and reputable websites.

| 🏗️ Continuous Building Status | 📦 Continuous Packing Status | 🚀 Continuous Releasing Status |
| ----------------------------- | ---------------------------- | ------------------------------ |
| [![Continuous Building](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-building.yml/badge.svg)](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-building.yml) | [![Continuous Packing](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-packing.yml/badge.svg)](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-packing.yml) | [![Continuous Releasing](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-releasing.yml/badge.svg)](https://github.com/jonathanlinat/quake-leveldesign-starterkit/actions/workflows/continuous-releasing.yml) |

Two artifacts are released, offering compatibility with the following operating systems:

> [!WARNING]
> Only 64-bit versions are supported.

- **Microsoft Windows**
- **Linux** (specifically for Debian-based distributions)

---

## Features

The current version of **QLDSK** includes the following set of tools and extras:

### Tools

* **ericw-tools**, Eric Wasylishen [[GitHub](https://github.com/ericwa/ericw-tools)] [[Website](https://ericwa.github.io/ericw-tools)]
  - A suite of command-line utilities for building levels (maps) for games like Quake and Hexen 2 represents an evolved branch of Tyrann's original Quake tools. The tools focus on adding advanced lighting features, some of which are borrowed from q3map2, and include bugfixes for the qbsp tool, which is used for constructing the block structure of the map.
* **Ironwail**, Andrei Drexler [[GitHub](https://github.com/andrei-drexler/ironwail)] [[Twitter](https://twitter.com/andrei_drexler)] 
  - An advanced fork of QuakeSpasm, a popular source port of the Quake engine, aimed at enhancing performance and introducing additional features. It has been optimized for high performance, incorporating modern techniques such as culling, GPU-accelerated lightmap updates, and compute shaders, allowing it to handle highly detailed Quake maps at high framerates.
* **Quake CLI Tools**, Joshua Skelton [[GitHub](https://github.com/joshuaskelly/quake-cli-tools)] [[Usage](https://www.youtube.com/watch?v=zJ0RX62VYaA)] [[Website](https://joshua.itch.io/quake-tools)] [[Discord](https://discord.gg/PyqRPNwnk7)]
  - A collection of command-line utilities to facilitate the creation of content for the Quake game series. These tools can perform various tasks, including managing PAK and WAD files, adding and extracting files, converting BSP files to WAD files, and even creating SVG files from BSP files.
* **TrenchBroom**, Kristian Duske [[GitHub](https://github.com/TrenchBroom/TrenchBroom)] [[Website](http://kristianduske.com/trenchbroom)] [[Discord](https://discord.gg/txsKc3EARW)]
  - A free, open-source, cross-platform level editor designed explicitly for Quake-engine-based games. It is compatible with games like Quake, Quake 2, and Hexen 2 and can be run on multiple operating systems. It is recognized for its ease of use, offering simple and advanced tools that enable designers to craft complex and engaging levels without much hassle.

### Extras

* **Prototype WAD**, Aleksander Marhall [[Source](https://www.slipseer.com/index.php?resources/prototype-wad.263)]
  - A resource containing Quake textures designed for map prototyping. It features 273 prototype textures that are indexed to Quake's palette. The collection includes basic checker textures in eight base colors, three shades, and four sizes (16x16, 32x32, 64x64, and 128x128). It also contains solid color textures, which include fullbright colors and specialized textures.
* **TrenchBroom Quake Map Source**, Atul Varma [[Source](https://book.leveldesignbook.com/appendix/resources/quake)]
  - A collection of the original Quake 1 MAP source files, as released by John Romero in 2006. These files have been converted to a modern format compatible with TrenchBroom. The texture references in these files have also been fixed with a repackaged `quake101.wad` file.

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
 
| 💬 Do You Need Support? |
| ----------------------- |
| [![](https://dcbadge.vercel.app/api/server/dh29D3kqrM?style=plastic)](https://discord.gg/dh29D3kqrM) |

### Software Requirements

* A legitimate copy of Quake [[Steam](https://store.steampowered.com/app/2310)] [[Good Old Games](https://www.gog.com/game/quake_the_offering)]
* For **Microsoft Windows** users:
  - Microsoft Visual C++ Redistributable for Visual Studio 2015, 2017 and 2019 [[x64](https://aka.ms/vs/16/release/vc_redist.x64.exe)]

### Download

Get the [latest ZIP release](https://github.com/jonathanlinat/quake-leveldesign-starterkit/releases) and extract its contents into a directory, likely named `quake-leveldesign-starterkit-[date]-[os]`.

---

## First Setup

1. Locate and open the `quake-leveldesign-starterkit-[date]-[os]` directory in your file explorer.
2. Create three new directories:
   - An `id1` directory inside the `game` directory.
   - A `maps` directory within the `id1` directory stores compiled maps.
   - A `working` directory at the root level will initially be empty. This directory will host `.map` files and other related files once the `ericw-tools` compiler is used.
3. Copy the `.pak` file(s) from your Quake game installation into the `id1` directory:
   - `pak0.pak` and `pak1.pak` from the original game release.
   - `pak0.pak` from the re-release.

> [!NOTE]
> These instructions also apply to other expansions and modifications.

Your directory structure should look like this:

```text
.
├── extras/
├── game/
│   └── id1/
│       ├── maps/
│       └── pak0.pak
│       └── (pak1.pak)
├── level-editor/
├── working/
└── tools/
```

> [!WARNING]
> For Unix system users: Grant execution rights to binaries.
>
> To set execution permissions recursively from the **QLDSK** directory, execute the following command in your Terminal: `find . -type f -exec sh -c 'file -b "{}" | grep -q "^ELF"' \; -exec chmod +x "{}" \;`.

### Configure the Quake Game Profile

1. Open `TrenchBroom`.
1. In the `Welcome to TrenchBroom` window, click on `New map...`.
1. In the `Select Game` window, click `Open preferences...`.
1. Select the `Quake` profile in the `Games` tab of the `Preferences` window.
1. Set the `Game Path` to `/path/to/quake-leveldesign-starterkit-[date]-[os]/game`.
1. Click on `Configure engines...`.
1. Add a new profile by clicking the `+` button.
1. Set `Name` to `Ironwail`.
1. Set `Path` to `/path/to/quake-leveldesign-starterkit-[date]-[os]/game/ironwail(.exe)`.
1. Click `Close`.
1. Leave the `Compilation Tools` fields empty.
1. Click `Apply`, then `OK`.
1. Select the `Quake` profile in the `Select Game` window.
1. Keep `Map Format` as `Valve`.
1. Click `OK`.

A new document is now open for mapping.

### Set Up the Compiler

1. Save the document in `/path/to/quake-leveldesign-starterkit-[date]-[os]/working`. Name it as you wish.
1. Click on the `Run` menu.
1. Select `Compile Map...`.
1. In the `Compile` window, add a new profile by clicking the `+` button.
1. Set `Name` to `Compile`.
1. Set `Working Directory` to `${MAP_DIR_PATH}`.
1. Add an `Export Map` task profile by clicking `+`.
1. Set `Field Path` to `${WORK_DIR_PATH}/${MAP_BASE_NAME}-compile.map`.
1. Add a `Run Tool` task profile for each of the following tools, setting `Tool Path` to the respective paths in `/path/to/quake-leveldesign-starterkit-[date]-[os]/tools/ericw-tools/bin/`:
    - `qbsp(.exe)` with `Parameters`: `-nocolor ${MAP_BASE_NAME}-compile.map ${MAP_BASE_NAME}.bsp`.
    - `vis(.exe)` with `Parameters`: `-nocolor ${MAP_BASE_NAME}.bsp`.
    - `light(.exe)` with `Parameters`: `-nocolor ${MAP_BASE_NAME}.bsp`.
    - `bspinfo(.exe)` with `Parameters`: `${MAP_BASE_NAME}.bsp`.
1. Enable `Stop on nonzero error code` for each tool.
1. Add a `Copy Files` task profile for each of the following files, setting `Target Directory Path` to `${GAME_DIR_PATH}/${MODS[-1]}/maps`:
    - `Source File Path` to `${WORK_DIR_PATH}/${MAP_BASE_NAME}.bsp`.
    - `Source File Path` to `${WORK_DIR_PATH}/${MAP_BASE_NAME}.lit`.
1. Ensure the tasks are all enabled.
1. Click on `Compile` and verify that everything works and the document compiles successfully.
1. Click on `Launch...`.
1. In the `Launch Engine` window, set `Parameters` to `-basedir /path/to/quake-leveldesign-starterkit-[date]-[os]/game/ +map <name-of-the-saved-document>`.
1. Click `Close`.

Congratulations! You are now ready to start mapping.

### References

To assist you in effectively configuring the tools included in this kit, consider these two informative articles for additional guidance:

> [!NOTE]
> The procedures outlined might vary slightly from the current project structure.

* **Setting up TrenchBroom in Ubuntu to create and compile Quake maps**, s3thra [[Website](https://quake.blog/trenchbroom-ubuntu-setup-tutorial.html)]
* **Configure TrenchBroom in Windows to create Quake maps**, s3thra [[Website](https://quake.blog/configure-trenchbroom-in-windows.html)]

---

## Getting Started

The inspiration for this project primarily comes from the excellent series of video tutorials by [dumptruck_ds](https://twitter.com/david_spell). Be sure to watch these [informative videos](https://www.youtube.com/playlist?list=PLgDKRPte5Y0AZ_K_PZbWbgBAEt5xf74aE)!

<p align="center"><a href="https://www.youtube.com/watch?v=gONePWocbqA" align="center"><img src="https://img.youtube.com/vi/gONePWocbqA/0.jpg"></a></p>

---

## Additional Resources

* **The Level Design Book**, Robert Yang [[Website](https://book.leveldesignbook.com)]
  - This online resource compiles a wealth of information on 3D video game-level design in a contemporary and accessible manner. It caters to designers across all levels of experience and various game engines.
* **Quaddicted**, Spirit [[Website](https://www.quaddicted.com)]
  - A fan site dedicated to the iconic game Quake, renowned for its comprehensive archive of Quake single-player maps. The site also includes installation tools, a range of archives featuring engines, tools, wads, multiplayer maps, and informative articles catering to the needs of both Quake players and developers.
* **Slipgate Sightseer**, Michael Markie [[Website](https://www.slipseer.com)]
  - A website dedicated to the Quake modding community. It offers a variety of content related to Quake, a popular first-person shooter game known for its modding capabilities and active community support. The site features tools and resources for both players and modders of Quake.
* **Quake.blog**, s3thra [[Website](https://quake.blog)]
  - A comprehensive blog that began as a platform to document the creator's experiences with TrenchBroom, Quake map creation, and playing Quake map packs. The blog has grown to include various content, including tutorials, personal stories, and videos, extending beyond the realm of Quake to cover other topics as well.
* **Func_Msgboard**, John Fitzgibbons [[Website](https://www.celephais.net)]
  - A significant forum and online community focused on video game-level design, particularly for Quake engine games. For over twenty years, it has been a central hub for hobbyist and professional-level designers to exchange ideas and discuss game development.
* **Quaketastic** [[Website](https://www.quaketastic.com)]
  - Hosts an extensive collection of reusable resources through a comprehensive file browser.

---

## Acknowledgments

A heartfelt thank you to **Devin 'shark' Smigle**, from the Discord channel [Quake Mapping](https://discord.gg/dh29D3kqrM), for his outstanding contribution, brilliantly bringing the project's vision to life with his unique creativity in the illustration! 👏

---

## License

**Quake Level Design Starter Kit**, also known as **QLDSK**, and its infrastructure is [CC0 1.0 Universal licensed](LICENSE).

The licenses of the compiled and released tools vary and are independent of **QLDSK**'s licensing. There is no guarantee that all tools will work perfectly in every scenario, and users should use them at their discretion.
