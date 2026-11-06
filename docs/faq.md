# The Godfather II Mods FAQ

Common questions about gf2mod and its mods for The Godfather 2 on PC.

**Where do I download gf2mod and the mods?**
On [Patreon](https://www.patreon.com/c/gf2mod). This repository contains only documentation and images.

**How do I install mods for The Godfather 2?**
Extract gf2mod into the game folder, add the mods and press **PLAY**. See the
[installation guide](getting-started.md).

**How do I increase the crew limit in The Godfather II?**
Use [Bigger Crew](mods/bigger-crew.md), which raises it from 3 to 20 by default, and up to 127.

**How do I get more made men in my family?**
Use [Bigger Family Tree](mods/bigger-family-tree.md), which grows your family from 7 to 10 made men.

**Do I need the manager?**
Yes. Every mod is a `.gf2mod` package that the [manager](manager.md) checks and applies.

**Does it change my game files?**
No. Delete the gf2mod files and the game is back to normal. See [how to remove it](getting-started.md#remove).

**Why is there a `d3d9.dll`?**
It's how the game loads the mods, the same way it loads tools like ReShade. It forwards everything else to the real Direct3D 9 of
Windows. See [how it works](manager.md#how-it-works).

**Which version of the game do I need?**
Version 1.0.789, the latest official patch. To check it, right-click `godfather2.exe` and open **Properties > Details**.

**A mod says it was made for another version. What now?**
Check your game version first. The message says which version the mod expects and which one you have.

**Can I use ReShade at the same time?**
Not in its d3d9 mode, because both need to be `d3d9.dll`. See [Compatibility](compatibility.md#other-tools).

**Can I use my `.asi` plugins?**
Yes, 32-bit ones. Put them in the `plugins` folder; you don't need a separate ASI loader.

**Can I use only part of a mod?**
Yes. Most mods are split into modules that you can turn off one by one in the manager.

**The game doesn't behave as expected. What should I send?**
The file `logs\gf2mod.log`, along with what you did and which mods were active. If the game closed, `logs\gf2mod-crash.dmp` helps
too.
