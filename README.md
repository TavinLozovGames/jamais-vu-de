# Jamais Vu

**A detective RPG system for Foundry VTT — in the spirit of Disco Elysium.**

Twenty-four skills that argue with you. Thoughts that take days to cook in the back of your head. A Loop that tightens every time you fail. A case board, an evidence journal, a city map full of pins, and a GM console built for two game masters working side by side.

Made by two people, for free, on pure enthusiasm.

[![Foundry](https://img.shields.io/badge/Foundry%20VTT-v12%2B-orange)](https://foundryvtt.com/)
[![Verified](https://img.shields.io/badge/verified-v14-success)](https://foundryvtt.com/)
[![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE)
[![Languages](https://img.shields.io/badge/languages-8-informational)](#languages)
[![Discord](https://img.shields.io/badge/Discord-join-5865F2)](https://discord.gg/BsDzQmS3SB)

![The detective sheet](docs/img/sheet-overview.png)
*The detective sheet: four attributes, twenty-four skills, morale, health, tokens and the case tracker — all on one screen.*

---

## Install

**In Foundry:** Setup → **Game Systems** → **Install System** → paste this into the *Manifest URL* field:

```
https://github.com/TavinLozovGames/jamais-vu-de/releases/latest/download/system.json
```

**Manually:** download `jamais-vu.zip` from [Releases](https://github.com/TavinLozovGames/jamais-vu-de/releases), unzip it into your Foundry user data folder under `Data/systems/`, so the path ends up as `Data/systems/jamais-vu/system.json`. Restart Foundry.

Then create a world with **Jamais Vu** as its system and log in as GM.

> **Requires Foundry VTT v12 or newer.** Verified on v14.

---

## What's in the box

- **24 skills across 4 attributes** — Intellect, Psyche, Physique, Motorics — each one a voice with its own opinion
- **White, yellow and red checks** — 2d6 + skill, with a check registry that remembers what's locked forever and what reopens as you grow
- **The Thought Cabinet** — thoughts cook over time, penalising the skill that whispers them until they ripen into a bonus
- **The Loop** — a doom clock that fills on failed checks and passing hours, and throws incidents at the table when it hits its thresholds
- **Investigation board** — nodes, threads and theories you can pull open in front of the players, one card at a time
- **Case journal and city map** — pins on the Foundry canvas, dossiers behind each one, revealed at your pace
- **NPC generator and oracle** — sparks when you're stuck mid-session
- **Reputation and factions**, shops, containers, Item Piles support
- **57 conditions** with modifiers, durations and icons
- **Light combat** — no initiative grind; weapons are modifiers, damage is small, the fight is a scene
- **A narrative character creator** — the "Awakening" text quest
- **Eight interface languages**, each player picks their own

---

## The detective sheet

![Skills](docs/img/sheet-skills.png)
*Twenty-four skills grouped under four attributes. Base value, modifiers from gear and thoughts, and the total you actually roll. Click a skill name to roll it.*

![Roll dialog](docs/img/roll-dialog.png)
*The roll dialog: pick the difficulty, add a situational modifier, choose white or red. 2d6 + skill against the number — snake eyes always fail, double sixes always succeed.*

![Status and conditions](docs/img/sheet-status.png)
*The lower half of the sheet: active conditions, effects, tags and notes. Conditions carry their own skill modifiers and durations.*

![Inventory](docs/img/sheet-inventory.png)
*Inventory — weapons, armour, clothing, tools, drugs. Equipped items feed their modifier straight into the relevant skill.*

![Thought Cabinet](docs/img/sheet-thought-cabinet.png)
*The Thought Cabinet. A thought that's cooking penalises its voice-skill and whispers into chat whenever you roll that skill — that's how it ripens. Once it's done, the penalty flips into a bonus.*

![Quests](docs/img/sheet-quests.png)
*Quests with stages and triggers. Name an item as a trigger and picking it up advances the quest by itself.*

![Sleep and Fight](docs/img/sheet-sleep-fight.png)
*Sleep closes the day, heals, and lets thoughts finish cooking. Fight opens the combat panel.*

---

## Making a detective

![The Awakening](docs/img/awakening-quest.png)
*The "Awakening" — a narrative text quest instead of a stat spreadsheet. Fifteen questions build your skills, then you choose a worldview.*

![Appearance](docs/img/awakening-appearance.png)
*Appearance, rolled or chosen: face, build, clothes, the small ruined details.*

![Portrait prompt](docs/img/awakening-portrait-prompt.png)
*At the end you get a finished sheet, a personal item, and a ready-made portrait prompt in the right style.*

![Create player](docs/img/codex-create-player.png)
*The GM codex handles the boring half: create the player actor, hand it over, and let them run the Awakening themselves.*

---

## Worldviews

Seven political stances, each with two bonuses and a cost: communism, socialism, ultranationalism, moralism, ultraliberalism, nihilism, and no ideology at all. Changing your mind costs a story trigger, a night's sleep and 3 XP — and while you're rethinking it, you get the penalty without the bonus.

---

## The Loop

![The Loop](docs/img/loop-dashboard.png)
*The Loop is pressure made visible. It fills on failed checks and on every phase of the day you burn through. At roughly 40% and 75%, and again when it closes, it throws an incident into the city — unrelated to your case, and entirely your problem.*

Six phases of the day — Dawn, Morning, Midday, Evening, Night, Deep Night — each one able to fire its own Foundry playlist automatically. Name a playlist after a phase, drop your tracks in, and the system handles the rest.

---

## Running the case

![Investigation board](docs/img/investigation-board.png)
*The investigation board: nodes for clues, people and places, threads between them, theories you can colour-code.*

![Board opened to players](docs/img/investigation-board-open.png)
*Open the board to the players — or reveal it card by card, an eye at a time.*

![Case journal](docs/img/case-journal.png)
*The case journal fills itself as things are revealed. Players see only what you've unlocked; the GM sees everything.*

![Check registry](docs/img/check-registry.png)
*The check registry logs the checks that matter. A failed white check reopens once the skill grows; a yellow one waits on a condition; a red one is locked forever.*

---

## The city

![Case map](docs/img/case-map.png)
*Clues and places of the case, listed beside the map. Click one to open its dossier, click again to zoom the canvas to it.*

![Add a marker](docs/img/map-add-marker.png)
*Markers live directly on the Foundry scene. Pick a glyph, drop it, and it lights up when the players find it — or stays dim until they do.*

![World map](docs/img/world-map.png)
*The whole city at once. Districts, the port, the river — pinned and lit as the investigation spreads.*

![Location sheet](docs/img/location-sheet.png)
*Locations are actors too: art, points on their own map, and transitions to neighbouring places for quick travel.*

![Scene sheet](docs/img/scene-sheet.png)
*Scenes hold read-aloud text, hooks and leads. "Read to players" pushes it to chat and marks the scene as reached.*

---

## People

![NPC sheet](docs/img/npc-sheet.png)
*The NPC dossier: what they know, how they break, what they're hiding, and how their voice sounds in dialogue.*

![NPC generator](docs/img/npc-generator.png)
*Out of ideas mid-session? Roll a stranger — gender, estate, role, age, politics, first impression, manner of speech, and a starting condition.*

![Factions and reputation](docs/img/factions-reputation.png)
*Five estates with their own standing toward the detective. Dockers, old money, the uniforms, the money-men, and the street.*

![Trade](docs/img/shop-trade.png)
*Shops and trade: stock, prices, wallet. Buy a coat, buy a bottle, buy a favour.*

![Containers](docs/img/container.png)
*Containers — desks, crates, corpses' pockets. Works with Item Piles if you have it installed.*

![Item browser](docs/img/item-browser.png)
*A base of ready items you can spawn from presets, plus 120 pieces of stock gear in the compendium.*

---

## Fighting

![Combat](docs/img/combat.png)
*Combat is a scene, not a spreadsheet. Equip a weapon, pick point-blank or at range, roll the skill it uses — on a hit, damage minus the target's armour. Health runs 0–5, so one bad decision matters.*

---

## GM tools

![GM console](docs/img/gm-console.png)
*The GM console, built for two game masters at once: a shared GM scene, a dispenser that feeds text to the players chunk by chunk, and a private GM channel.*

![Oracle](docs/img/oracle.png)
*The oracle: yes/no with complications, twists, names, places, and case sparks — all in the tone of a post-war port city.*

![Voices](docs/img/voices.png)
*Skill voices — interjections in the Disco Elysium idiom, posted to chat under the skill that's speaking.*

![Speaking queue](docs/img/speaking-queue.png)
*A speaking queue and sound controls, so the table doesn't talk over itself.*

![Big chat](docs/img/big-chat.png)
*A full-size chat window for when the sidebar isn't enough — read-aloud text deserves room.*

![Export and import](docs/img/export-import.png)
*Export and import the whole case — board, journal, markers, factions — to carry it between worlds or back it up.*

---

## Languages

![Language select](docs/img/language-select.png)

The interface ships in **English, Русский, Українська, Čeština, Deutsch, Français, Español and Polski**. Each player picks their own language on first launch and it's remembered in their browser — the GM can run in one language while the table reads another.

Some long-form text (condition descriptions, gear flavour, incident text) currently falls back to English outside EN and RU. Translation help is very welcome — see [Contributing](#contributing).

---

## First steps for a GM

1. Create a world on the Jamais Vu system and log in as GM.
2. Open the **Codex** (the system's GM panel) and create a Detective actor for each player, then assign it to their user.
3. Have each player run the **Awakening** to build their detective.
4. Import the gear and thoughts compendiums if you want the stock content.
5. Create Foundry playlists named after the day phases if you want automatic ambience.
6. Open the **Dashboard**, set the Loop length for your case, and start the day.

---

## Contributing

Bug reports and feature requests go in [Issues](https://github.com/TavinLozovGames/jamais-vu-de/issues) — there are templates for both.

**Translations** are the easiest way to help. Copy `lang/en.json`, translate the values (leave the keys alone), and open an issue or a pull request. Missing keys fall back to English automatically, so a partial translation is still useful.

---

## Credits

Built by **Tavin & Lozov**.

Based on the *Jamais Vu* homebrew ruleset. Inspired by the writing, structure and voice of **Disco Elysium**.

---

## Support

This is a free project made in our spare time. If you want it to keep growing, any coin helps:

- 💛 [Monobank jar](https://send.monobank.ua/jar/9kSDeyUQ9q)
- 💬 [Discord](https://discord.gg/BsDzQmS3SB) — questions, bug reports, and tables looking for players

---

## License

Code is released under the [MIT License](LICENSE).

Artwork, icons and written game text remain the property of their authors and are licensed for use with this system only — see `LICENSE` for the exact terms.

---

## Disclaimer

*Jamais Vu* is an unofficial, non-commercial fan project. It is not affiliated with, endorsed by, or sponsored by ZA/UM, and it contains no assets from *Disco Elysium*. All trademarks belong to their respective owners.
