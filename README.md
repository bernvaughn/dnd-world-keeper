# dnd-world-keeper

A tracker for my Dungeons & Dragons worlds. Each world is a separate game played with a different group, and they never mix.

## Worlds

| Slug | Game | Setting |
|------|------|---------|
| [`vpl`](worlds/vpl/README.md) | Vassalboro Public Library game | Faerun (homebrewed from Forgotten Realms) |
| [`kee`](worlds/kee/README.md) | Keenan's Tuesday game | Sead and Xianhua |

## Structure

```
AGENTS.md              agent instructions and conventions
skills/                reusable agent skills (index in skills/README.md)
worlds/
└── <world>/
    ├── README.md      world overview
    ├── characters/
    │   ├── pcs/       player characters, with full detail
    │   └── npcs/      non-player characters, with full detail
    ├── sessions/      session logs and recaps
    ├── factions/      organizations and groups
    ├── items/         notable items
    └── continents/
        └── <continent>/
            ├── README.md
            ├── locations/        points of interest outside cities
            └── cities/
                └── <city>/
                    ├── README.md
                    └── locations/    shops, taverns, points of interest
```

## Conventions

- Every folder's overview is a `README.md`, so GitHub renders it when browsing.
- File and folder names are lowercase kebab-case slugs (for example `old-mill-tavern`).
- Full character detail lives only in the world-level `characters/pcs/` and `characters/npcs/` folders. Locations list the characters found there with a short blurb and a relative link back.
- This is a public repo, so real player names are never recorded. Player characters are referred to by character name only.
- Session files are named `session-YYYY-MM-DD.md`.

See [AGENTS.md](AGENTS.md) for the full rules agents follow when working in this repo.
