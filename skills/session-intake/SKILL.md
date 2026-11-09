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
   - session log: `sessions/session-YYYY-MM-DD-dmN.md`
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

- This is a public repo. Never record real player names or anything that could identify the people at the table. Refer to characters by character name only. Pasted notes may map players to characters, or mention who attended, swapped characters, or stopped coming. Use the character names only and leave out everything about the players, including in your own replies where possible.
- The library game has many players and several DMs playing different quests in one shared world, so different sessions can involve different parties.
- Session files are named by the date played and the DM code: `session-YYYY-MM-DD-dmN.md`. DM codes (`dm1`, `dm2`, `dm3`, and so on) are opaque. Never record which person a code belongs to, and never use initials or names. The owner keeps that mapping outside the repo and may forget it, so in each new chat ask whose session is whose before naming a file. When a new DM comes up, ask, then assign the next unused code. All sessions recorded before codes were introduced are `dm1`.

## Discord messages

The owner may paste Discord messages from a game and ask for details to be filled in from them.

- Infer each message batch's session date from its timestamps, and tell the owner the guess. Timestamps may not line up exactly with the session date.
- Keep Discord-sourced details clearly marked "from Discord messages", separate from the owner's own notes. Do not merge them into the session story as fact.
- Where Discord and existing notes conflict, flag the conflict and change nothing.
- Leave out Discord handles, player names, and anything that could identify the people at the table. Use character names only.
- Follow the same steps as above: post the file list and questions first, then wait for an explicit go.
- Keep what the owner said. Do not restructure the repo or add top-level folders without asking.
