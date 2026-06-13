    # Nova Modding Suite
Discord: https://discord.gg/Z6P23hjEsM
**A visual, crash-safe creation hub for Hearts of Iron IV mods.** Build focus trees, research, events, decisions, national spirits, characters, country setups, and a full map — without hand-writing a single line of Paradox script.

Nova sits on top of the base game (or any mod, like Millennium Dawn) and writes **only to your own mod** — vanilla and the mods you depend on are never touched. Every tool runs its edits through a Save-gate that refuses or warns on the things that crash HOI4 on launch, so you find problems in the editor instead of at a black screen.

> Not affiliated with or endorsed by Paradox Interactive. Hearts of Iron IV is a trademark of Paradox Interactive.

---

## What's inside

| Tool | What it does |
|------|--------------|
| **Country Setup** | Create a new country or customize an existing one — ideology, ruling party, national spirits, capital (picked on the map), starting tech. |
| **Focus Tree** | Drag-and-drop focus-tree designer with a deep effect/trigger engine and a live plain-English ("Genesis") preview of what each focus actually does. |
| **Research Tree** | Add custom technology tabs, techs, and equipment, rendered 1:1 with the in-game grid. Scope a tab to a specific country. |
| **Event Maker** | Author events with options, triggers, MTTH/typed fire dates, and effects. |
| **Decision Maker** | Decision categories and missions with costs, timers, and effects. |
| **National Spirits** | Country ideas/spirits with modifiers, equipment bonuses, and AI hints. |
| **Characters** | Country leaders, advisors, generals and admirals with traits and portraits. |
| **Map Editor** | Edit state ownership, cores, manpower, buildings, resources and victory points; move provinces; strategic regions; supply areas; terrain/coastal; and paint province shapes. |
| **Mod Health** | One-click validation with a health score, grouped issues, deep-links to the right maker, and safe auto-fixes. |

**✦ Genesis** turns your scripted content into plain English everywhere, so you can read a focus, spirit, or decision back like a sentence instead of a wall of tokens.

**🛡️ Crash-safe by design.** The map editor's Save-gate blocks the documented HOI4 launch-crash causes before they reach your mod — provinces in two states, a state or supply area split across strategic regions, factories over the category's building slots, a country annexed out of its capital, a sea province inside a state, a missing/typo'd state category, and more.

---

## Requirements

- **Windows** (the portable build is x64).
- **Hearts of Iron IV** installed — Nova reads the base-game assets, localization, and detects `hoi4.exe`.
- **Node.js 18+** only if you run from source or build locally.

Nova auto-detects your game and mods under the usual Steam / Documents paths. You can override detection with environment variables:

| Variable | Purpose |
|----------|---------|
| `HOI4_MOD_ROOT` | Absolute path to the mod folder you want to edit (the one containing `descriptor.mod`). |
| `HOI4_ROOT` | Absolute path to the game install containing `hoi4.exe`. |
| `PORT` | Port for the embedded server (default `47821`). |

---

## How it works

Nova runs a small local server that reads the merged game data (base game → dependencies → your mod, the same way HOI4 loads it) and serves the editors in a desktop window. Saves are written **only** to your active mod, with atomic writes and `.bak` backups, so a crash mid-save can never corrupt a file.

---

## Contributing

Issues and pull requests are welcome. If you hit a crash, the in-app diagnostics bundle the game's logs and the newest crash dump into one report — attach that.

## License

See [LICENSE](LICENSE). Hearts of Iron IV game files are © Paradox Interactive and are not redistributed by this project.

    

