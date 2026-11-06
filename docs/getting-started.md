# How to Install Mods for The Godfather II (PC)

This guide explains how to install gf2mod and its mods for The Godfather 2 on PC, how to configure them and how to remove them.

## Requirements

- **The Godfather II for PC, version 1.0.789**, the latest official patch. To check it, right-click `godfather2.exe` and open
  **Properties > Details**. The original 1.0.764 release is not supported.
- **Windows 10 or 11.**

## Install

1. Download gf2mod and the mods you want from [Patreon](https://www.patreon.com/c/gf2mod).
2. Extract the gf2mod archive into the game folder, where `godfather2.exe` is. You get `gf2mod.exe`, `d3d9.dll` and the `mods`,
   `plugins` and `logs` folders.
3. Put the `.gf2mod` files of your mods into the `mods` folder, or drop them onto the gf2mod window.
4. Start `gf2mod.exe`, tick the mods you want and press **PLAY**.

After the first PLAY you can also start the game from its usual shortcut: your last selection stays applied.

## Configure

Select a mod in the window to see its parts (called *modules*) and its options. Changes apply the next time you press **PLAY**.
Each mod's page lists its modules and options:

- [Bigger Crew](mods/bigger-crew.md)
- [Recruitable Soldiers](mods/recruitable-soldiers.md)
- [Bigger Family Tree](mods/bigger-family-tree.md)
- [Minimap Icons](mods/minimap-icons.md)

## Remove

Delete `gf2mod.exe`, `d3d9.dll`, `gf2mod.ini` and the `mods`, `plugins` and `logs` folders from the game folder. No game file is
ever modified. Before removing a mod you use in a saved game, read [Compatibility](compatibility.md#save-games).

## If something goes wrong

Open `logs\gf2mod.log`. It lists every mod and module, what was applied and the reason if something was not. Please include it
when you report a problem.
