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
│   ├── pcs/                        # player characters
│   └── npcs/                       # non-player characters
├── sessions/
├── factions/
├── items/
├── ships/
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
- **Character detail lives in one place:** `worlds/<world>/characters/pcs/<slug>.md` (player characters) and `worlds/<world>/characters/npcs/<slug>.md` (non-player characters) hold all detailed character information. A location file lists the characters found there with a one-line blurb and a relative link to the character file. Do not duplicate character detail in locations.
- **This is a public repo:** never record real player names or anything that could identify the people at the table. Refer to player characters by character name only.
- **Sessions:** named `session-YYYY-MM-DD.md` by the date played.
- **Unknowns:** when something is not recorded, write "not recorded" instead of guessing. Keep open questions visible.
- **Links:** use relative links between files, for example `../../../../../characters/npcs/mara-voss.md` from a city location file. Keep slugs short, since links get long at this depth.
- **Cities** are folders (`cities/<slug>/README.md` plus `cities/<slug>/locations/`). **Locations** are single files unless they need to grow into a folder.
- **Empty folders** hold a `.gitkeep`. Delete it once real content is added.

## Working rules

- Do not invent lore, characters, or rules and present them as established. When filling a gap, ask the owner or mark the text clearly as a proposal.
- Preserve the owner's wording and decisions when editing existing files.
- Do not create new top-level folders or restructure the layout without asking.
- When the owner pastes session notes, follow [skills/session-intake/SKILL.md](skills/session-intake/SKILL.md). Never write files before the owner has approved the plan.
- Reusable agent skills go in `skills/`. Add them only when the owner asks, and list each in `skills/README.md`.
