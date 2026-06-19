# Discord forum — first post (copy into `#plugins`)

**Title:** `MapKillCounter`

**Tags:** `community`

---

## MapKillCounter

**Author:** MordWraith  
**Source:** https://github.com/MordWraith/MapKillCounter  
**Compatible with:** [Gordin/GameHelper2](https://github.com/Gordin/GameHelper2) `main`, **.NET 10** (`net10.0-windows`, x64). Works on maintained community forks on the same API/target.

### What it does (PoE2)

Map and session **kill counter** for GameHelper:

- Kills by rarity: **N**ormal, **M**agic, **R**are, **U**nique (compact labels)
- **Map timer** + optional **session overlay** (totals across maps)
- Timer pauses in town/hideout, on ESC pause menu, when game is in background (configurable)
- Horizontal or vertical layout, resizable overlay, custom colors

Read-only overlay — no input automation.

### Install (source only — no prebuilt DLL)

1. Clone [GameHelper2](https://github.com/Gordin/GameHelper2)
2. Clone this plugin into `Plugins/MapKillCounter`:
   ```
   git clone https://github.com/MordWraith/MapKillCounter.git Plugins/MapKillCounter
   ```
3. Build:
   ```
   dotnet build GameHelper/GameHelper.csproj -c Release
   dotnet build Plugins/MapKillCounter/MapKillCounter.csproj -c Release
   ```
4. Enable **MapKillCounter** in GameHelper → Plugins

Full README: https://github.com/MordWraith/MapKillCounter

### Config folder

- `config/settings.txt` — overlay layout, timers, colors (JSON)

### v1.0.0

- Initial community release

### Support

- Feedback / feature requests: **this thread**
- Crashes / GameHelper install issues: `#help` with tag **`plugin`**

### Disclaimer

Community third-party plugin. Use at your own risk. Not affiliated with GGG. Only install from trusted sources.

---

## Update checklist (for you)

When releasing a new version, edit this first post:

1. Bump version in `MapKillCounter.csproj` and README version table
2. Add bullet under **vX.Y.Z** with changes
