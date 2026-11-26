# LegionCore — Reforged development tracker

Live page: https://titans-project.github.io/

The page shows the state of each part of [LegionCore — Reforged](https://github.com/Titans-Project/LegionCore-Reforged), the World of Warcraft: Legion 7.3.5 server emulator.

## Updating a status

Everything the page shows comes from `status.json`. To change a status, edit the matching line and change the `updated` date at the top.

Each entry looks like this:

```json
{ "name": "Return to Karazhan", "status": "untested", "note": "optional short text" }
```

`status` is one of `working` (green), `partial` (yellow), `progress` (orange), `broken` (red, not working) or `untested` (grey). Artifact weapon quests and world bosses also carry a `group` (the class) or a `detail` (specialization, zone). An optional `also` shows a second status next to the first one (for example `broken` with `"also": "progress"`); only `status` is counted.

The page is in English and French: `name_fr`, `detail_fr`, `group_fr`, `note_fr` and `title_fr` hold the French text, and the English one is shown when they are missing.

A section with `"layout": "feature"` (Legion events) shows each entry as a row with a picture (`image`), an optional map icon in its corner (`icon`) and a short description (`desc`, `desc_fr`).
