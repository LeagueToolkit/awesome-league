<div align="center">
<h1>Awesome League</h1>

A curated list of tools, libraries, and resources for working with League of Legends files, assets, and mods

</div>

## Table of Contents

- [File Format Index](#file-format-index)
- [Mod Managers](#mod-managers)
- [Modding](#modding)
- [WAD Archives](#wad-archives)
- [Bin & Property Files](#bin--property-files)
- [Textures & Images](#textures--images)
- [3D Models & Animation](#3d-models--animation)
- [VFX & Materials](#vfx--materials)
- [Audio](#audio)
- [Hashtables](#hashtables)
- [Game Manifests](#game-manifests)
- [Misc](#misc)
- [Libraries](#libraries)
- [Documentation](#documentation)

<!-- -------------- FORMAT INDEX -------------- -->
## File Format Index

Not sure where to look? Find your file format here:

| Format | What it is | Where to look |
| --- | --- | --- |
| `.wad`, `.wad.client` | Game asset archives | [WAD Archives](#wad-archives) |
| `.bin` | Object/property data (characters, skins, VFX, ...) | [Bin & Property Files](#bin--property-files) |
| `.tex`, `.dds` | Textures | [Textures & Images](#textures--images) |
| `.skn`, `.skl`, `.anm`, `.scb`, `.sco` | Meshes, skeletons, animations | [3D Models & Animation](#3d-models--animation) |
| `.bnk`, `.wpk` | Audio soundbanks | [Audio](#audio) |
| Shader bytecode | Compiled shaders | [Misc](#misc) |
| `.fantome`, `.modpkg` | Mod packages | [Modding](#modding) |
| Hashes, `.hashdb` | Hash → path tables for resolving file names | [Hashtables](#hashtables) |
| Manifests | Game file download data | [Game Manifests](#game-manifests) |

<!-- -------------- MOD MANAGERS -------------- -->
## Mod Managers

Trusted mod managers for installing and running mods.

- [LTK Manager](https://github.com/LeagueToolkit/ltk-manager) `GUI` - The official LeagueToolkit mod manager, succeeding the original cslol-manager
- [cslol-go](https://github.com/Aurecueil/Cs-lol-go) `GUI` - Mod manager bundled with the Topaz mod fixer

<!-- -------------- MODDING -------------- -->
## Modding

Creating, fixing, and distributing mods.

- [Flint](https://github.com/LeagueToolkit/Flint) `GUI` - Modding IDE for extracting, previewing, editing, and exporting League assets
- [Hematite](https://github.com/LeagueToolkit/Hematite) `CLI` - Automatically detects and fixes common issues in custom League skins
- [league-mod](https://github.com/LeagueToolkit/league-mod) `CLI` - Toolkit for creating, managing, and distributing League of Legends mods
- [League-Mod-Repather](https://github.com/RitoShark/League-Mod-Repather) `GUI` - Automatically repaths `.fantome` files and mod folders; also fixes issues like square particles and game crashes
- [LtMAO](https://github.com/tarngaina/LtMAO) `GUI` - Collection of various tools and utilities to help modders
- [TopazModFixerCLI](https://github.com/LeagueToolkit/TopazModFixerCLI) `CLI` - Standalone CLI for the Topaz mod fixer (C#), used in Cslol-go and available for automation and integration into other tools

<!-- -------------- WAD -------------- -->
## WAD Archives

Exploring, extracting, and building `.wad` game archives.

- [hexbelt](https://alanpq.github.io/hexbelt) `Web` - Web app for exploring/interacting with `.wad` & `.bin` files
- [Obsidian](https://github.com/Crauzer/Obsidian) `GUI` - Tool for exploring and extracting `WAD` files with a modern UI
- [wadtools](https://github.com/LeagueToolkit/wadtools) `CLI` - High-performance tool for extracting and working with WAD files; includes modern automatic hash management, file diffing and scanning 

<!-- -------------- BIN -------------- -->
## Bin & Property Files

Converting and editing `.bin` property files and their legacy predecessors.

- [hexbelt](https://alanpq.github.io/hexbelt) `Web` - Web app for exploring/interacting with `.wad` & `.bin` files
- [lolpytools](https://github.com/moonshadow565/lolpytools) `CLI` - Python scripts for converting inibin, troybin, luaobj and luabin files
- [ritobin](https://github.com/moonshadow565/ritobin) `CLI` - Converts League's `.bin` format to a human-readable version (`.ritobin`)
- [ritobin-lsp](https://github.com/alanpq/ritobin-lsp) `LSP` - The official LSP server for the `.ritobin` language format; includes formatting, auto-complete and linting of structs using an integration with the LTK meta wiki database
- [ritobin-tools](https://github.com/LeagueToolkit/ritobin-tools) `CLI` - CLI tool for working with Ritobin (`.py`/`.bin`) files

<!-- -------------- TEXTURES -------------- -->
## Textures & Images

Converting and editing `.tex` and `.dds` texture files.

- [ltk-tex-utils](https://github.com/LeagueToolkit/ltk-tex-utils) `CLI` - Robust converter for `.tex` files; convert back and forth between common image formats
- [Ritoddstex](https://github.com/Morilli/Ritoddstex) `CLI` - Simple converter for dds<->tex files

### Image Editor Plugins

- [Gimp-Tex-Plugin](https://github.com/RitoShark/Gimp-Tex-Plugin) `Plugin` - Open and save League of Legends `.tex` files in GIMP
- [ltk-tex-thumb-handler](https://github.com/LeagueToolkit/ltk-tex-utils) `Plugin` - Show `.tex` texture previews in Windows Explorer
- [Paint.NET-Tex-Plugin](https://github.com/RitoShark/Paint.NET-Tex-Plugin) `Plugin` - Import and save `.tex` files in Paint.NET, with Windows Explorer previews
- [RitoTex-Photoshop](https://github.com/LeagueToolkit/RitoTex-Photoshop) `Plugin` - Load and save `.tex` texture files in Photoshop

<!-- -------------- 3D -------------- -->
## 3D Models & Animation

Importing, exporting, and converting meshes, skeletons, and animations.

- [Aventurine-League-Tools](https://github.com/RitoShark/Aventurine-League-Tools) `Plugin` - Blender plugin for League of Legends asset import/export
- [lemon3d](https://github.com/tarngaina/LtMAO#lemon3d) `Plugin` - Modern and maintained iteration of the Autodesk Maya plugin, bundled with the LtMAO app
- [lol2gltf](https://github.com/Crauzer/lol2gltf) `CLI` - Convert 3D assets from League into the glTF format (partial support for converting glTF to League formats as well)

<!-- -------------- VFX -------------- -->
## VFX & Materials

Editing particles, materials, and recoloring effects.

- [Chroma-Tool-Studio](https://github.com/VISION4RIO/chroma-tool-studio) `GUI` - Edit `.dds` files using full color instead of pixels and recolor VFX in one click by tracking relevant values in code
- [Quartz](https://github.com/RitoShark/Quartz) `GUI` - All-in-one VFX & material editor

<!-- -------------- AUDIO -------------- -->
## Audio

Extracting and building `.bnk`/`.wpk` soundbanks.

- [bnk_gui](https://github.com/Morilli/bnk-extract-GUI/releases) `GUI` - Audio soundbank editor
- [Wwise](https://www.audiokinetic.com/en/wwise/overview/) `GUI` - Audiokinetic's audio middleware, used to make custom soundbanks
- [Wwiser](https://github.com/bnnm/wwiser) `CLI` - Analyze `_events.bnk` files

<!-- -------------- HASHTABLES -------------- -->
## Hashtables

Hash → path tables for resolving the game's hashed file and field names.

- [League Hashes by CDragon](https://github.com/CommunityDragon/Data) - Actively maintained collection of hashes used by League
- [mimir](https://github.com/LeagueToolkit/mimir) `CLI` - Toolkit for generating, storing, and serving League hash → path tables as a compact, memory-mapped binary format (`.hashdb`)

<!-- -------------- MANIFESTS -------------- -->
## Game Manifests

Manifests for downloading game files from Riot's CDN.

- [ManifestDownloaderGUI](https://github.com/dazashu/ManifestDownloaderGUI) `GUI` - Download Riot manifest files
- [riot-manifests](https://github.com/Morilli/riot-manifests) - List of manifest files for Riot Games products, including League

<!-- -------------- MISC -------------- -->
## Misc

- [shader-tools](https://github.com/LeagueToolkit/shader-tools) `CLI` - CLI tool for extracting shader bytecode

<!-- -------------- LIBRARIES -------------- -->
## Libraries

For developers building their own tools.

- [cdragon-rs](https://github.com/CommunityDragon/cdragon-rs) `Rust` - CDragon Rust library collection
- [league-toolkit](https://github.com/LeagueToolkit/league-toolkit) `Rust` - Rust implementation of League Toolkit
- [LeagueToolkit](https://github.com/LeagueToolkit/LeagueToolkit) `C#` - Parse, edit and convert various League of Legends file formats
- [pyritofile](https://github.com/GuiSaiUwU/pyritofile-package) `Python` - Python package to deal with League of Legends files

<!-- -------------- DOCS -------------- -->
## Documentation

- [LTK Wiki](https://wiki.leaguetoolkit.dev/) - The official LeagueToolkit wiki - the main hub for League modding knowledge and documentation of the LeagueToolkit ecosystem, created by people who've been here since the beginning of modding
- [lol-meta-classes](https://github.com/LeagueToolkit/lol-meta-classes) - Tracks League's `.bin` meta class metadata across updates - all existing and past classes/properties in the game, including their default values, in a custom database
- [lol-meta-wiki](https://github.com/sxrmss/lol-meta-wiki) - Wiki for documenting League of Legends Meta `.bin` classes and properties
