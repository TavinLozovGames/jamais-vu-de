# Contributing

Jamais Vu is made by two people in their spare time. Help is genuinely welcome, and small help is still help.

## Reporting a bug

Open an [issue](https://github.com/TavinLozovGames/jamais-vu-de/issues) using the bug template.

The single most useful thing you can include is the **console output**: press `F12` in Foundry, open the Console tab, and copy any red lines. Most bugs are solved from that alone.

## Suggesting a feature

Open an issue with the feature template. Describe it from the table's point of view — what should happen in play — rather than how you think it should be coded. We'll figure out the code.

## Translating

This is the easiest and most valuable way to help.

1. Take `lang/en.json` as your source.
2. Translate the **values**. Leave the **keys** exactly as they are.
3. Send it back as a pull request, or just attach the file to an issue — either is fine.

Things worth knowing:

- **Partial translations are useful.** Any key you leave out falls back to English automatically, so you can start with the sheet and the buttons and leave the long condition descriptions for later.
- **Watch the length.** Some strings sit in narrow buttons and tabs. If a translation runs long, shorten it rather than let it overflow.
- **Some strings are deliberately not translated.** The oracle tables are GM-facing content and stay as they are. A few internal labels are matched against playlist names in code and must not change — they're marked in the file.
- Machine translation is fine as a first pass, but a native speaker needs to read it before it ships. If you're that speaker, say so in the issue.

Current state: English and Russian are complete. Ukrainian, Czech, German, French, Spanish and Polish cover the interface but fall back to English for long descriptions.

## Contributing code

Fork, branch, pull request. A few house rules:

- The system is a **single file** — `jamais-vu.mjs`. That's deliberate for now, while the campaign it was built for is still running. Please don't submit a PR that splits it into modules.
- **Never call `game.i18n.localize()` or `.format()` in top-level data** — in a `const` outside a function. `game.i18n` doesn't exist yet when the module loads, and it takes the whole system down with it. Store the key in the data and localise where it's displayed.
- A new map marker glyph must be added to **both** `JV_MAP_MARKERS` and `JV_MARK_UNI`, or it renders as an empty circle.
- Full-screen elements with `mix-blend-mode` destroy framerate. We've already tried.
- Before submitting: `node --check jamais-vu.mjs` should pass, Handlebars tags should balance, and the language JSON files should still parse.

## Contributing art

Talk to us first on [Discord](https://discord.gg/BsDzQmS3SB) before you spend time on anything.

Two constraints, both non-negotiable:

- It has to be **your own work**, and you have to be able to say so. Generated images can't go into the package.
- It has to fit the visual language: flat opaque planes, sparse dark accents, strong figure-ground separation at the silhouette edge.

## What we can't accept

Our campaign setting, its city, its cast and its mystery are not part of this project and won't be published. Please don't send setting material expecting it to be merged — Jamais Vu is an engine, and what you run on it is yours.

## Credit

Everyone who contributes is credited in the release notes and in the welcome window. If you'd rather not be, say so and we'll leave you out.
