# Changelog

## gf2mod manager

### 1.1.0

- ASI plugins: put any `.asi` plugin in the new `plugins` folder and gf2mod loads it, with no separate ASI loader.
- Plugins load at game start, before Direct3D, so plugins that hook Direct3D work as expected.
- Each plugin has its own on/off box in the window, and can be installed or removed from there.
- New setting in `gf2mod.ini`: `[General] Plugins=0` turns all plugins off at once.
- 64-bit plugins and files that aren't plugins are refused, and the window says why, instead of crashing the game.
- A plugin already loaded by another ASI loader isn't loaded twice.

### 1.0.1

- Fixed: mods were refused with "made for another version of godfather2.exe" on a normal 1.0.789 game.
- Mods now check the game version, and the message says which version is expected and which one you have.

### 1.0.0

- First release: mod manager window, per-mod modules and options, and package checks.

## Mods

| Mod | Version | Notes |
|---|---|---|
| Bigger Crew | 1.0.1 | Updated to the new game version check. |
| Recruitable Soldiers | 1.0.1 | Updated to the new game version check. |
| Bigger Family Tree | 1.0.1 | Updated to the new game version check. |
| Minimap Icons | 1.0.0 | First release. |
