# Agent Instructions

This repo tracks the owner's Dungeons & Dragons worlds. Read this file before making any change.

## The worlds

- `worlds/vpl/` is the Vassalboro Public Library game. Its continent is Faerun. The setting started from Forgotten Realms but has grown into its own thing, so published canon is only a starting point. Treat what is written in this repo as the truth, and record places where it diverges from canon.
- `worlds/kee/` is Keenan's Tuesday game. Its continents are Sead and Xianhua.

Each world is a distinct game played with different people. Never mix characters, places, factions, items, or events between worlds. If a request is ambiguous about which world it concerns, ask.

## Layout

```
worlds/<world>/
├── README.md
├── characters/
├── sessions/
├── factions/
├── items/
└── continents/<continent>/
    ├── README.md
    ├── locations/                  # points of interest outside cities
    └── cities/<city>/
        ├── README.md
        └── locations/              # shops, taverns, points of interest
```

## Conventions

- **Overviews:** every folder's overview is a `README.md`.
- **Names:** lowercase kebab-case slugs for every file and folder (`old-mill-tavern.md`, `port-vale/`).
- **Character detail lives in one place:** `worlds/<world>/characters/<slug>.md` holds all detailed character information. A location file lists the characters found there with a one-line blurb and a relative link to the character file. Do not duplicate character detail in locations.
- **Links:** use relative links between files, for example `../../../../../characters/mara-voss.md`. Keep slugs short, since links get long at this depth.
- **Cities** are folders (`cities/<slug>/README.md` plus `cities/<slug>/locations/`). **Locations** are single files unless they need to grow into a folder.
- **Empty folders** hold a `.gitkeep`. Delete it once real content is added.

## Working rules

- Do not invent lore, characters, or rules and present them as established. When filling a gap, ask the owner or mark the text clearly as a proposal.
- Preserve the owner's wording and decisions when editing existing files.
- Do not create new top-level folders or restructure the layout without asking.
- Reusable agent skills go in `skills/`. Add them only when the owner asks, and list each in `skills/README.md`.
