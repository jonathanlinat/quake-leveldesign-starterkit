<p align="center"><img src="https://github.com/jonathanlinat/quake-leveldesign-starterkit/assets/14064112/03402bb0-65fe-4b86-a95d-3b92aeb044b7"></p>
<h1 align="center">Quake Level Design Starter Kit</h1>

**Quake Level Design Starter Kit**, also known as **QLDSK**, consolidates various tools and resources into one comprehensive package, facilitating the quick and easy creation of **Quake** and **GoldSrc** engine-based maps with just a few clicks.

![qldsk-preview](https://github.com/user-attachments/assets/2ac3a477-f00e-4de9-a5e5-2d572f3cc259)

---

## Releases

| 🚀 Get the Latest Stable Release | 🔔 Get the Latest Weekly (Unstable) Release |
| -- | -- |
| [![Get the Latest Stable Release](https://badgen.net/github/release/jonathanlinat/quake-leveldesign-starterkit?icon=github&label=Release)](https://github.com/jonathanlinat/quake-leveldesign-starterkit/releases/tag/v20241231-f8dfdd6897) | [![Get the Latest Weekly Release](https://badgen.net/github/release/jonathanlinat/quake-leveldesign-starterkit?icon=github&label=Release)](https://github.com/jonathanlinat/quake-leveldesign-starterkit/releases/latest) |

Great, you're all set! Now, proceed to [read the documentation](https://github.com/jonathanlinat/quake-leveldesign-starterkit/wiki) to install, set up and start this project.

| 💬 Do You Still Need Support? |
| -- |
| [![](https://dcbadge.vercel.app/api/server/dh29D3kqrM?style=plastic)](https://discord.gg/dh29D3kqrM) [![](https://dcbadge.vercel.app/api/server/BXEjbQYdnC?style=plastic)](https://discord.gg/BXEjbQYdnC) |

---

## Features

The current version of **QLDSK** includes the following set of applications, tools and extras:

### Applications

* **TrenchBroom**, Kristian Duske [[GitHub](https://github.com/TrenchBroom/TrenchBroom)] [[Website](http://kristianduske.com/trenchbroom)] [[Discord](https://discord.gg/txsKc3EARW)]
   - A free, open-source, cross-platform level editor designed explicitly for Quake engine-based games. It is compatible with games like Quake and Half-Life and can be run on multiple operating systems. It is recognized for its ease of use, offering simple and advanced tools that enable designers to craft complex and engaging levels without much hassle.
* **ericw-tools**, Eric Wasylishen [[GitHub](https://github.com/ericwa/ericw-tools)] [[Documentation](https://ericw-tools.readthedocs.io)]
   - A suite of command-line utilities for building levels (maps) for games like Quake and Half-Life represents an evolved branch of Tyrann's original Quake tools. The tools focus on adding advanced lighting features, some of which are borrowed from [q3map2](http://q3map2.robotrenegade.com/), and include bugfixes for the `qbsp` tool, which is used for constructing the block structure of the map.

### Tools

* **Ironwail**, Andrei Drexler [[GitHub](https://github.com/andrei-drexler/ironwail)] [[Twitter](https://twitter.com/andrei_drexler)] 
   - An advanced fork of QuakeSpasm, a popular source port of the Quake engine, aimed at enhancing performance and introducing additional features. It has been optimized for high performance, incorporating modern techniques such as culling, GPU-accelerated lightmap updates, and compute shaders, allowing it to handle highly detailed Quake maps at high framerates.
* **Quake CLI Tools**, Joshua Skelton [[GitHub](https://github.com/joshuaskelly/quake-cli-tools)] [[Usage](https://www.youtube.com/watch?v=zJ0RX62VYaA)] [[Website](https://joshua.itch.io/quake-tools)] [[Discord](https://discord.gg/PyqRPNwnk7)]
   - A collection of command-line utilities to facilitate the creation of content for the Quake game series. These tools can perform various tasks, including managing `.pak` and `.wad` files, adding and extracting files, converting `.bsp` files to `.wad` files, and even creating `.svg` files from `.bsp` files.
* **goldutil**, Léo Peltier [[GitHub](https://github.com/L-P/goldutil)]
   - A comprehensive suite of GoldSrc engine CLI utilities for content creation, offering `.wad` and `.spr` files management, entity graph generation, and `.map` file cleanup to streamline TrenchBroom workflows.

### Extras

#### Quake

* **Prototype WAD**, Aleksander Marhall [[Slipseer](https://www.slipseer.com/index.php?resources/prototype-wad.263)]
   - A resource containing Quake textures designed for map prototyping. It features 273 prototype textures that are indexed to Quake's palette. The collection includes basic checker textures in eight base colours, three shades, and four sizes (16x16, 32x32, 64x64, and 128x128). It also contains solid colour textures, including fullbright and specialized textures.
* **Quake Palette**, Spiney [[Quake Wiki](https://quakewiki.org/wiki/Quake_palette)]
   - The original Quake's palette provided in multiple formats: `.lmp`, `.aco`, `.act`, `.ase`, `.pal`, `.png` and `.txt`.
* **TrenchBroom Quake Map Source**, Atul Varma [[The Level Design Book](https://book.leveldesignbook.com/appendix/resources/quake)]
   - A collection of the original Quake `.map` source files, as released by John Romero in 2006. These files have been converted to a modern format compatible with TrenchBroom. The texture references in these files have also been fixed with a repackaged `quake101.wad` file.

#### GoldSrc

* **Digit's Developer Textures**, Digit404 [[GameBanana](https://gamebanana.com/mods/6693)]
   - A curated set of simplified, unobtrusive developer textures designed specifically for map developers, simplifying the process of scene blocking by eliminating the need for texture selection. These textures enhance focus on the layout and structural aspects, facilitating a more productive and uninterrupted mapping experience. Especially suitable for beginners.

---

## License

**Quake Level Design Starter Kit**, also known as **QLDSK**, and its infrastructure is [CC0 1.0 Universal licensed](LICENSE).

The licenses of the compiled and released tools vary and are independent of **QLDSK**'s licensing. There is no guarantee that all tools will work perfectly in every scenario, and users should use them at their discretion.
