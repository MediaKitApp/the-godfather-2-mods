# gf2mod: Mod Manager for The Godfather II (PC)

<img src="../assets/gf2mod/poster.webp" alt="gf2mod, the mod manager for The Godfather II on PC" width="100%">

**Version 1.1.0.** [Download gf2mod on Patreon](https://www.patreon.com/c/gf2mod).

gf2mod is the mod manager and launcher for The Godfather 2 on PC, and every mod here needs it. Install, enable and configure
`.gf2mod` packages from one window. It also loads ASI plugins and adds a windowed mode.

## Features

- **Clean dark-themed window:** mod list, modules and options of each mod, and a **PLAY** button.
- **Full control:** turn whole mods or single modules on and off and change their options, without touching any file.
- **Easy install:** drag and drop, or use the *Install mod...* button. Remove with one click.
- **ASI plugins:** put a `.asi` plugin in the `plugins` folder and gf2mod loads it, with its own on/off box. Only 32-bit plugins
  work, like the game. Tested with *Carmine Family Revival* and *GF2_MiniMapPlus*.
- **Package checks:** a package for a different game version, or a damaged file, is refused with a clear message.
- **Windowed mode:** Direct3D 9 ignores the game's brightness in a window; gf2mod applies it, so the window no longer looks
  darker.
- **Clear log:** `logs\gf2mod.log` lists every mod and module, what was applied and the reason if something was not.

## How it works

The game loads `d3d9.dll` from its own folder, as it does with ReShade or DXVK. gf2mod builds that single DLL from its runtime and
the mods you enabled, and the DLL forwards everything else to the real Direct3D 9 of Windows.

- Nothing is injected into other programs and nothing is downloaded.
- No game file is changed. Mods that alter the game's interface carry only a small patch, applied in memory when the game loads
  the original.
- The only code loaded while the game starts, besides that DLL, is the ASI plugins you put in `plugins`. gf2mod can't check what a
  plugin changes.
- Every release is scanned with an antivirus (Kaspersky) before upload.

## Console commands

For advanced users, `gf2mod.exe` also works from a console:

| Command | What it does |
|---|---|
| `gf2mod list` | Lists the installed mods. |
| `gf2mod install <file>` | Checks and installs a `.gf2mod` package or `.asi` plugin. |
| `gf2mod info <mod>` | Shows modules and options with their current values. |
| `gf2mod enable <mod or file.asi>` | Turns a mod or plugin on. `disable` turns it off. |
| `gf2mod module <mod> <module> on` | Turns one module on or `off`. |
| `gf2mod set <mod> <Section.Key> <value>` | Changes an option, checking its type and range. |
| `gf2mod window on` | Starts the game in a window, or `off` for fullscreen. |
| `gf2mod build` | Generates `d3d9.dll` without starting the game. |
