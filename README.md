# MapKillCounter

Community plugin for [GameHelper2](https://github.com/Gordin/GameHelper2) (Path of Exile 2).

Per-**map** and per-**session** monster kill counts by rarity (**N/M/R/U**), map timer, optional session overlay, horizontal or vertical layout. Written by **MordWraith** for community forks. Read-only overlay — **build from source**.

## Features

- Kill counts: Normal, Magic, Rare, Unique (compact **N/M/R/U** labels)
- **Map timer** and optional **session timer** (pauses in town/hideout, on ESC, when game in background)
- Resizable overlays, custom colors, font scale
- Session overlay for totals across maps

## Requirements

- A working [GameHelper2](https://github.com/Gordin/GameHelper2) source tree
- **.NET 10 SDK** (`net10.0-windows`, x64)

## Build & install

```bash
git clone https://github.com/Gordin/GameHelper2.git
cd GameHelper2
git clone https://github.com/MordWraith/MapKillCounter.git Plugins/MapKillCounter
dotnet build GameHelper/GameHelper.csproj -c Release
dotnet build Plugins/MapKillCounter/MapKillCounter.csproj -c Release
```

Enable **MapKillCounter** in GameHelper → Plugins.

### Config folder

| Path | Purpose |
|------|---------|
| `Plugins/MapKillCounter/config/settings.txt` | Overlay layout, timers, colors (JSON) |

## Credits

- Author: **MordWraith**
- Built for [GameHelper2](https://github.com/Gordin/GameHelper2) (Gordin / community)

## Disclaimer

Third-party plugin — use at your own risk. Read-only overlay; no automation.

## Version history

| Version | Notes |
|---------|--------|
| **1.0.0** | Initial community release: map/session kills, timers, N/M/R/U layout |
