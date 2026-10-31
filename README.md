<div align="center">

# 📖 The Holy Earth Foundation — Reading room, public

*The proposals, procedures and decks the foundation is ready to show, with a front end at*
***<https://theholyearthfoundation.github.io/reading-room-public/>***

![Room](https://img.shields.io/badge/Room-public-d97706?style=flat-square)
![Allowlist](https://img.shields.io/badge/Allowlist-empty-6b4f1d?style=flat-square)
![Edits](https://img.shields.io/badge/Edits-by_sync_only-b45309?style=flat-square)
![For](https://img.shields.io/badge/For-Visitors-64748b?style=flat-square)

</div>

---

## 🧭 What this is

The foundation's members read drafts in a private reading room. When an officer decides a page is ready for
visitors, it is added to that room's allowlist and copied here, and this repository's GitHub Pages site lists it on a
shelf. Until then the shelves say where each piece waits.

## 🌱 What is here

| File | Owned by | What it does |
|---|---|---|
| `index.html`, `assets/`, `.nojekyll` | this repository | the front end: one static page in the foundation's amber, no build step, readable on a phone, light and dark |
| `README.md` | this repository | this page |
| `room-manifest.json` | the sync | the list of files the sync copied, read by the front end (absent until the first sync) |
| `proposals/`, `procedures/`, `decks/` | the sync | only the paths an officer has allowlisted (none yet) |

## 🔒 How it is kept

- **Nobody edits the synced folders by hand.** The private room's sync copies exactly its allowlisted paths after a
  tripwire that stops anything that looks like a credential, an internal note or a personal matter, and commits them
  here as an ordinary commit. The front end's own files are never overwritten by it.
- `main` cannot be deleted (a deletion-only ruleset). Pages builds from `main`, at the root.
- To change the front end, open a pull request here; to change what is published, change the allowlist in the private room.

## 🙋 Reading the members' room

Members of the foundation send their GitHub username to the steward or to Kenney, accept the invitation, and read the
private room in a browser. The page's *Read the members' room* section has the steps.

## 🔗 Elsewhere

- [🏠 The foundation →](https://theholyearthfoundation.github.io)
- 📋 The procedures' public twin: [`ops-standard-operating-procedures-public`](https://github.com/theholyearthfoundation/ops-standard-operating-procedures-public)
- 📜 The lab's public proposals preview: [`drasticstatic/proposals-thef-public-preview`](https://github.com/drasticstatic/proposals-thef-public-preview)
