# VanaCoreXIV

Dalamud control panel for FFXIV (FOV/zoom, UI scale & theme, graphics config, presets, optional post-process helpers, mod-pack listing, in-plugin VFX path hide).

Inspired by FFXI VanaCore-style *control*, built for **FFXIV + Dalamud** — not a 1:1 port.

## Install (plugin)

1. Dalamud → Settings → Experimental → Custom plugin repositories  
2. Add your `pluginmaster.json` raw URL (GitHub)  
3. Install **VanaCoreXIV** from the Plugin Installer  

Or load `VanaCoreXIV.dll` + `VanaCoreXIV.json` from a release zip (**only those two files** in the Dalamud plugin zip).

Open with: `/vanacore`

## What the plugin does

- Camera (opt-in), UI scale/theme, SystemConfig graphics, presets  
- Optional **Penumbra**: list `.pmp` / `.ttmp` under `ModPacks\` and enable/disable via Penumbra when Penumbra is installed  
- **In-plugin VFX path hide** (EasyEyes-style) — does **not** require EasyEyes or VFXEditor  
- DoF: **native-first** where the game allows; full GPose DoF is still Group Pose  

## Optional: ReShade (not required for core plugin)

ReShade / `game_drop` is **optional** (bloom/clarity/extra post).

- Download `game_drop.zip` if provided  
- Put `VanaCoreBridge.addon64` next to `ffxiv_dx11.exe`  
- Put `VanaCoreDriver.fx` in `reshade-shaders\Shaders\`  
- **Do not** put `.addon64` inside the Dalamud plugin zip — Dalamud will not use it  

## Optional: glow packs

Carbuncle/fairy look changes from **`.pmp` packs** still need **Penumbra** (or TexTools → Penumbra).  
VanaCore can list packs and, when Penumbra is present, help enable them. It does not replace Penumbra as a full mod loader.

## Notes

- Third-party tools (EasyEyes, VFXEditor, ReShade) are optional companions, not required for basic `/vanacore` features  
- No redistribution of Square Enix game files or other authors’ mod packs in this repo’s plugin zip  
