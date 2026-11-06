# The Godfather II Mod Compatibility

What works with gf2mod and its mods for The Godfather 2 on PC: game version, other tools and save games.

## Game version

gf2mod and its mods support **The Godfather II for PC, version 1.0.789**. The original 1.0.764 release is not supported. The
manager checks the version and tells you which one a mod expects and which one you have.

## Other tools

- **Tools that replace `d3d9.dll`**, such as ReShade or ENB in d3d9 mode, can't be used at the same time.
- **ASI plugins** work through the `plugins` folder, 32-bit only. gf2mod can't check what a plugin changes. A plugin already
  loaded by another ASI loader isn't loaded twice.
- **Other minimap dot plugins:** turn one off when using [Minimap Icons](mods/minimap-icons.md), or you get two dots per person.

## Between mods

The mods are designed to work together. If two of them ever try to change the same part of the game, the second change is refused
and written to the log instead of crashing the game.

[Recruitable Soldiers](mods/recruitable-soldiers.md) recommends [Bigger Crew](mods/bigger-crew.md).

## Save games

| Mod | What to know |
|---|---|
| Bigger Crew | Saving and loading with more than 3 crew members has not been tested much yet. Please report any problem. |
| Recruitable Soldiers | No specific notes yet. |
| Bigger Family Tree | Saves keep their normal format. If you remove the mod with more than 1 underboss, 2 capos or 4 soldiers, the extra members have no slot when the save loads. Keep the mod while you use those slots. |
| Minimap Icons | Nothing is stored in your save. Turn the mod off and the radar is back to normal. |
