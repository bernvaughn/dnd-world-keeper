---
name: session-intake
description: Turn the owner's raw D&D session notes into linked world files in this repo. Use when the owner pastes session notes or asks to add a session, city, character, faction, item, or ship from notes.
---

# Session intake

Turn raw session notes into files in `worlds/<world>/`, without guessing and without writing anything the owner has not approved.

## Steps

1. **Read first.** Read `AGENTS.md` for the layout and conventions, and the target world's `README.md`. Look at existing files so you reuse characters, places, and slugs instead of duplicating them.
2. **Identify the world.** `vpl` (library game, Faerun) or `kee` (Keenan's Tuesday game). Never mix them. If unclear, ask.
3. **Map the notes to files.** Decide which of these each fact belongs to:
   - session log: `sessions/session-YYYY-MM-DD.md`
   - PCs and NPCs: `characters/pcs/` and `characters/npcs/`
   - factions, items, and ships: `factions/`, `items/`, `ships/`
   - places: `continents/<continent>/cities/<city>/` and its `locations/`, or the continent's own `locations/`

   Character detail lives only in the character files. Locations link to characters.
4. **Ask questions before writing.** Post the planned file list and grouped questions in one message. Typical gaps:
   - continuity: which party, how this session relates to others, where it took place
   - classes, races, and spellings that are missing or inconsistent in the notes
   - NPC roles, ship types, and item properties
   - gold amounts, counts, and who got what
   - whether unnamed characters should be recorded or left unnamed

   Flag conflicts inside the notes, such as a premise that disagrees with the session events, instead of silently choosing one.
5. **Get approval.** Show the final file list and wait for an explicit go. Ask whether to commit straight to `main` or to a branch.
6. **Write the files.** Use lowercase kebab-case slugs and relative links between files. Write "not recorded" for anything the owner has not told you. Record the owner's spellings exactly, including intentional ones. Do not invent lore.
7. **Update the indexes.** Add new cities, locations, characters, factions, and sessions to the relevant `README.md` files, and remove `.gitkeep` files from folders that now have content.
8. **Check links.** Every relative markdown link must resolve before you commit.
9. **Commit and push.** Use a clear commit message, then confirm the remote matches.

## Rules

- This is a public repo. Never record real player names or anything that could identify the people at the table. Refer to characters by character name only.
- The library game has many players and several DMs playing different quests in one shared world, so different sessions can involve different parties.
- Session files are named by the date played: `session-YYYY-MM-DD.md`.
- Keep what the owner said. Do not restructure the repo or add top-level folders without asking.
