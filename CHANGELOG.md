**English** · [한국어](CHANGELOG.ko.md) · [日本語](CHANGELOG.ja.md) · [中文](CHANGELOG.zh.md)

# Changelog

Notable changes in public releases of Ancestor's Map. Versions use `major.minor.patch`; dates are calendar dates in Korea (UTC+9).
This follows the [Keep a Changelog](https://keepachangelog.com/en/1.1.0/) format, using New features, Improvements and Bug fixes.

There were no public releases for 1.0.0, 1.0.1 or 1.1.1; 1.0.2 was the first public release.

## [1.3.2] - 2026-11-01

### New features

- **Building navigation**: press Q / E or use the new buttons in a building window to switch to the previous or next building. Locked buildings are skipped, and the buttons follow the window's opening and switching animations.
- **Auto-switch at curios**: if your party includes an Antiquarian or a modded hero with bonus curio loot, the app selects that hero just before a curio that can yield loot. Turn it on or off beside that hero's health bar during exploration.
- **Speed settings (speed multipliers)**: the first button in the overlay side panel lets you adjust forward movement, backward movement, combat and scouting speeds separately. Reset or close the app to restore the original values.

### Improvements

- **Enemy spoiler controls**: when you hide enemy information using the battle icon below the map, enemy groups in newly spawned corridor battles also stay hidden until you encounter them, even in corridors you have already visited.
- **Trinket presets**: after applying a preset, the cursor moves to the trinket bag's close button.
- **Town meter**: opens briefly when you enter town, then folds to its header.
- **Auto torch**: if you select **Black as Pitch (0)**, it returns to the setting you used before that selection when the expedition ends.
- Minor UI adjustments.

### Bug fixes

- Various bug fixes.

## [1.3.0] - 2026-10-30

### New features

- **Party & trinket presets**: arrow button next to the first roster row on the quest select screen. Works with modded heroes and extra trinket slots. Suggested order: pick the quest → party preset → trinket preset
- **Random party**: dice button
- **Party name combos**: shows which named party combinations you have completed
- **Turn order**: switch between the confirmed order and predicted odds (every speed + 1d8 roll combination)

### Improvements

- **Stalling counter**: shows whether the selected skill prevents or triggers reinforcements
- **Overlay mode**: switches on when a save loads (you can still switch back to the standalone window); per-element toggles and a foldable side panel during expeditions
- Patched game executables are recognized
- Clearer notices.

### Bug fixes

- Various bug fixes.

## [1.2.0] - 2026-10-27

### New features

- Added **overlay mode**: the app draws its information right on the game screen, laid out like the game's own UI. Toggle it with <code>[ &#96; ]</code> or the diamond button (formerly "Hide screen").

### Bug fixes

- Various bug fixes.

## [1.1.4] - 2026-10-24

### New features

- Added info for skills that transfer specific effects.

### Improvements

- Added support for a tall, narrow add-on window layout.

### Bug fixes

- Various bug fixes.

## [1.1.3] - 2026-10-23

### Improvements

- The battle screen now shows the name of the selected skill with its icon above the center mark.
- Skills that push or pull an ally now show the move chance and destination rank above that ally.
- Auto torch use: Hover a light level on the bar to see that level's effects.

### Bug fixes

- Fixed dead heroes staying in the Heroes table.
- Fixed disease chances showing on heroes with the Crimson Curse. They can't catch other diseases, so it now shows 0%.
- Fixed stuttering when turns change in battle.
- Fixed enemy action prediction and some other calculations to match the game.

## [1.1.2] - 2026-10-21

### New features

- Riposte preview: On the battle screen, targets that will riposte show their riposte damage, hit, crit and effects below the attack numbers. The numbers stay on screen while the attack plays out.
- Auto torch use: Pick a light level on the bar above the light info, and the app lights a torch for you whenever the light drops below it while exploring. Pick Black as Pitch (0) to keep the light at 0 instead, even in battle.
- Ambush chance at camp: While camping, the scouting line shows the chance of a nighttime ambush. When a flashback battle, such as the Shieldbreaker's, is coming instead, it tells you that.

### Improvements

- Your settings are now saved.

### Bug fixes

- Fixed some calculations to match the game.

## [1.1.0] - 2026-10-17

### New features

- Battle screen: The map area turns into a battle screen during battles. It shows damage, hit, crit and effect chances for each target of your skill, the enemy's chosen skill and target, status durations and DoT damage.
- Pick from the card: Click a row on a curio, obstacle or hunger card to make that choice in the game.
- Traps: Exploring stops in front of scouted traps, and you can pick a hero on the trap card to disarm.
- Inventory sort and sell values: Press [I] while exploring to sort your inventory. Hover over the app's bag icon to see sell values.
- Your default party order is restored after each battle (toggle with the Party button).

### Improvements

- The screen guide has been rebuilt.

### Bug fixes

- Fixed trinket and quirk buff numbers not matching the game.
- Fixed colored keywords in game text losing their color.
- Fixed mod text sometimes showing in the wrong language.

## [1.0.8] - 2026-10-12

### New features

- Auto-buy: click a row in the supply table twice and the app clicks the store for you to buy up to the recommended amounts. Extras are sold back, free supplies from heroes are left alone, and your slots are tidied into store order afterwards. With The Crimson Court, it also packs blood for each cursed hero in the party (1 for Short, 2 for Medium, 3 for Long, 4 for Exhausting per cursed hero), leaving in the Estate the blood that heroes waiting in town need.

### Improvements

- The supply table now supports the Courtyard Plus, Farmstead Plus, Sunward Isles, Vermintide and The Fiend Festival mods. Their dungeons only show up when the mod is enabled. (These are estimates worked out from each mod's dungeon generation rules and curio weights, so they may not be exact.)
- On the provisioning screen, the quest you picked is highlighted and its dungeon moves to the top of the table.

### Bug fixes

- Debug F6 (reset stress) no longer counts as stress healing in the meter.
- Fixed some skill icons not showing for modded classes.
- Fixed extra blank space beside some hero sprites (Arbalest, Shieldbreaker).

## [1.0.7] - 2026-10-09

### New features

- You can now hide info the game doesn't give you. Click the battle or hunger icon in the bottom row.
  - Battle: special encounter locations and enemy lineups on tiles you haven't visited.
  - Hunger: hunger tiles on the map.
  - These settings work independently of "explored only" and persist between sessions.

## [1.0.6] - 2026-10-07

### New features

- Added a party-wide cumulative meter in town (counts expeditions from this update onward).
- Hover over a portrait in the hero table to see the hero's appearance, gear levels, combat skill levels and camping skills.

### Improvements

- The final meter is now shown at the bottom of the expedition log when an expedition ends.

## [1.0.5] - 2026-10-05

### Improvements

- A Shambler summoned at an altar now shows the Shambler marker on the map.

### Bug fixes

- Fixed combat cards not showing after some heroes died during an expedition.

## [1.0.4] - 2026-10-05

### Bug fixes

- Fixed a hero sometimes missing from the combat bar early in a new campaign (e.g. Dismas in the tutorial).

## [1.0.3] - 2026-10-05

### New features

- **Room travel from the app map**: click a connected room to move there in the game.
- **Obstacle card**: when you interact with an obstacle, shows the cost of clearing it by hand and the supplies needed to remove it.

### Bug fixes

- **More accurate expedition meter**
  - Riposte damage and kills now count for the hero who riposted.
  - Bleed, blight and burn damage and kills now count for the hero who applied them, including burn spread by Wildfire and Controlled Burn.
  - Heal over time now counts for the healer, even when it ticks in corridors.
  - Fixed the final blow on the last enemy sometimes going uncounted.
- Fixed enemy lineups missing from map tiles for encounters added by mods.

## [1.0.2] - 2026-10-04

### New features

- **New version notice** — Checks this repository for the latest release on launch and shows a notice when a new version is available. Click the signature at the top left for app info and manual update checks. It does not download or replace files automatically.
- **Screen guide** — The question-mark button at the top right explains each screen step by step.

### Bug fixes

- Various fixes, including combat-card light modifiers and expedition meter attribution.

[1.3.2]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.3.2
[1.3.0]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.3.0
[1.2.0]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.2.0
[1.1.4]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.1.4
[1.1.3]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.1.3
[1.1.2]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.1.2
[1.1.0]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.1.0
[1.0.8]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.0.8
[1.0.7]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.0.7
[1.0.6]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.0.6
[1.0.5]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.0.5
[1.0.4]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.0.4
[1.0.3]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.0.3
[1.0.2]: https://github.com/Eolaloe/DD-AncestorsMap/releases/tag/v1.0.2
