# LegionCore — Reforged development tracker

Live page: https://titans-project.github.io/

The page shows the state of each part of [LegionCore — Reforged](https://github.com/Titans-Project/LegionCore-Reforged), the World of Warcraft: Legion 7.3.5 server emulator.

## Updating a status

Everything the page shows comes from `status.json`. To change a status, edit the matching line and change the `updated` date at the top.

Each entry looks like this:

```json
{ "name": "Return to Karazhan", "status": "untested", "note": "optional short text" }
```

`status` is one of `working`, `partial`, `progress` or `untested`. Artifact weapon quests and world bosses also carry a `group` (the class) or a `detail` (specialization, zone).
