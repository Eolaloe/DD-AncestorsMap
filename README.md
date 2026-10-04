**English** · [한국어](README.ko.md) · [日本語](README.ja.md) · [简体中文](README.zh.md)

# Ancestor's Map — DD Field Guide

An overlay for Darkest Dungeon that puts **the dungeon map, combat numbers and an activity log the game never shows you** right on top of your game.
It stays on top even over a fullscreen game, and clicking it doesn't steal your input — the game keeps receiving it.

Nothing is hard-coded from vanilla. It **reads the base game, DLC and every mod enabled in your current save and merges them**, so curios, monsters, trinkets and quirks added or changed by mods show up with their real in-game values. Load a different save and it re-syncs on its own.

**[⬇ Download the latest version](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest)**

## What it does

- **Detailed map** — Laid out like the in-game map. Hover any tile for curios, traps, enemy groups and interaction results. **Shortest-route guidance** to quest curios, the boss and the Courtyard, a **provision tracker** for curios you haven't touched yet, scouting chance, exact light-level modifiers, and alerts for special encounters (Thing from the Stars, Fanatic, Shambler, Collector).
- **Combat info** — Accuracy, damage, crit and effect chance for every skill from every rank, which skill an enemy is likely to use and on whom, turn order, a stalling tracker (how many anti-reinforcement actions you've taken this round and what the next round will bring), and retreat odds.
- **Activity log & meter** — Combat, exploration and camping are logged automatically, and a meter compares each hero's kills, damage dealt and taken, healing and stress.
- **Database search** — Look up enemies, trinkets, town events, diseases, virtues, afflictions and quirks by name, rarity, class or effect. Modded entries included.
- **In the Hamlet** — **Recommended provisions** by dungeon and length, and a **cost calculator** for building and district upgrades (against what you own plus this expedition's haul).
- **Guided tour** — Press the **?** button in the top-right corner for a step-by-step tour of each screen (it uses a sample expedition, so it works in town too).

Some features reveal information the game deliberately hides. By default the map shows **only explored areas**; the full map is a toggle at the top. Turn order and the retreat outcome are on by default — click the title in the middle of the combat bar to turn them off.

<details>
<summary>Full feature list</summary>

### Map
- A detailed map shaped like the in-game one. Choose between explored areas only and the whole dungeon.
- Counts of remaining battles, curios, traps and hunger tiles, plus how many provisions your curios will need.
- Hover a tile to see the enemy group, which provisions a curio takes and what they do, trap and obstacle effects, whether hunger is about to hit, and secret rooms.
- Supports the Crimson Court's Courtyard maps.

### Routing, special encounters, light
- The **shortest route** to quest curios, the boss and the Courtyard.
- **Pinpoints** the Thing from the Stars and the Fanatic on the map, and shows **trigger conditions and odds** for the Collector and the Shambler.
- **Exact numbers** for every light-level effect: stress, scouting, surprise, dodge, crit, enemy accuracy and damage, and bonus loot.

### Combat
- This round's **turn order** for both sides, and whose turn it is right now.
- Hover a portrait for a **combat card**.
  - For heroes: accuracy, damage, crit and effect chance against each enemy rank — final values with trinkets, quirks, diseases and buffs applied, including hidden modifiers the game never displays.
  - For enemies: the same numbers against each hero rank, plus the odds of which skill they'll use and who they'll target.
  - Characters that change modes, like the Abomination or the Duelist, are shown in **their current mode** with that mode's skills.
- **Stalling** — Color-coded risk of reinforcements next round, and a live count of anti-reinforcement actions taken this round.
- **Retreat** — Success chance, and with turn order enabled, whether retreating right now will succeed.
- **Expedition meter** — Hover the title in the middle to compare each hero's kills, damage dealt, damage taken, HP healed, stress taken, stress healed and stuns this expedition. Camping skills, meals and item heals count too.

### Activity log
- Records everything that happens in combat and exploration, using the game's own wording and colors: skills, hits, damage, effects, resists, ripostes, heart attacks and act-outs, plus curios, traps, obstacles and hunger.
- Outcomes aren't guessed — it reads **the results the game itself displays**.
- Switches to the log when a battle starts and back to the map when it ends.
- One log per dungeon run; the last 10 per save are kept so you can look back.

### Hamlet
- **Recommended provision counts** for each dungeon and expedition length.
- **Database** — Search enemies, trinkets, town events, diseases, virtues, afflictions and quirks by any value.
- **Building & district costs** — Compares what a chosen upgrade tier needs against what you have (estate plus this expedition's loot). Effect text matches the game, and it's available mid-expedition too.

</details>

## Installation

1. Download `AncestorsMap.zip` from [Releases](https://github.com/Eolaloe/DD-AncestorsMap/releases/latest) and extract it anywhere.
2. Run `AncestorsMap.exe`. It needs the **.NET 8 Desktop Runtime** — if it's missing, Windows will point you to the installer.
3. Launch the game and the app finds your save automatically. On first run, take the tour with the **?** button.

## Requirements & compatibility

- Windows 10/11 and the [.NET 8 Desktop Runtime](https://dotnet.microsoft.com/download/dotnet/8.0).
- Live combat data (turn order, stalling, retreat, curio windows) requires running the game **as 64-bit**. Supported: the Steam public build and the coming_in_hot beta, with either the Steam or the DRM-free (`_windowsnosteam`) executable. On 32-bit or an unrecognized game version the app skips memory reading, **runs from your save alone**, and tells you why in the status line above the activity log.
- Mods are picked up automatically from the enabled list and load order in your save. Works alongside most mods that change game data (dungeon mods tested: Farmstead Plus, The Sunward Isles, Vermintide).
- Built and tested on the Steam version, and confirmed on the DRM-free executable. Other platforms such as GOG may store the game or saves elsewhere and might not be detected.
- English · 한국어 · 日本語 · 简体中文. It follows the game's language at first and uses the game's own translations for names and descriptions.

## Safety

- It **never writes** to your saves, game files or game memory, and never injects anything into the game (no hooks, no injection).
- Game memory is opened **read-only**. Saves are written a turn late and roll outcomes aren't saved at all, so memory is used only to keep combat info live. Unlike Cheat Engine, which finds values to **change** them, this only finds values to **show** them.
- The only network traffic is **one update check at startup** (a GitHub release lookup). No accounts, no keys, no data collection.
- Because it reads another program's memory, some antivirus software may flag it. You can verify your download against the SHA-256 in the release notes.
- Art and text are read from your game install. No game assets are bundled — the app is a single ~3.5 MB executable.

## Updates

When a new version is out, a notice appears when you start the app, and **Check for updates** opens this repository's release page. Nothing is downloaded or replaced automatically — just grab the new zip and overwrite. Click the signature in the top-left corner to see your current version and check for updates. Settings and expedition logs are kept in `%LocalAppData%\AncestorsMap`.

## Controls

| Key / mouse | Action |
|---|---|
| `` ` `` (above Tab) | Show / hide |
| `Caps Lock` | Presses the game's **Default Party Order** button (the game has no hotkey for it) |
| `Home` | Close the database, log or estate view and return to the map |
| Left-drag · right-drag | Move the window · pan the map |
| Wheel · wheel click | Zoom · switch between map and log |
| Drag window edge · top slider | Resize · opacity |
| **?** button · top-left signature | Guided tour · app info (version, update check) |

`` ` ``, `Caps Lock`, `Home` and wheel-clicking over the game **only work while the game window is in front**; everywhere else they behave normally.

## Known limitations

- Live data is only read on supported 64-bit game versions. After a game update, the app runs from saves alone until it's updated for the new version.
- The recommended provisions table combines the English wiki, community guides and the dungeon generation rules — treat it as a guide.
- Not every mod has been tested. If something looks off, please report it below.

## Reporting issues

Open an [issue](https://github.com/Eolaloe/DD-AncestorsMap/issues) and include:
- App version (click the signature, top left) and game version (Steam public / coming_in_hot / DRM-free)
- Your enabled mods, which screen you were on and what you did, and a screenshot if you can

## License & credits

[LICENSE](LICENSE) — free for personal use; redistribution only unmodified and with attribution; no selling.
Darkest Dungeon is a game by Red Hook Studios. This app doesn't include any game assets.
Made with help from Claude and ChatGPT.
