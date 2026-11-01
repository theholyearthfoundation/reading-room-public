<div align="center">

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/theholyearthfoundation/.github/main/profile/assets/banner-dark.svg">
  <img alt="The Holy Earth Foundation: the foundation's golden heart within a breathing halo, framed by a living vine. The banner moves gently; with reduced motion it shows still." src="https://raw.githubusercontent.com/theholyearthfoundation/.github/main/profile/assets/banner-light.svg" width="100%">
</picture>

# <img src="assets/icons/book-open.svg" width="32" height="32" alt=""> The Holy Earth Foundation — Reading room, public

*The proposals, procedures and decks the foundation is ready to show, with a front end at*
***<https://theholyearthfoundation.github.io/reading-room-public/>***

![Room](https://img.shields.io/badge/Room-public-d97706?style=flat-square)
![Allowlist](https://img.shields.io/badge/Allowlist-start_here_and_shared_procedures-6b4f1d?style=flat-square)
![Edits](https://img.shields.io/badge/Edits-by_sync_only-b45309?style=flat-square)
![For](https://img.shields.io/badge/For-Visitors-64748b?style=flat-square)

**[<img src="assets/icons/door-open.svg" width="16" height="16" alt=""> Members: enter the reading room](https://github.com/theholyearthfoundation/reading-room)** (sign in to GitHub first)

</div>

---

## <img src="assets/icons/compass.svg" width="24" height="24" alt=""> What this is

The foundation's members read drafts in a private reading room. When an officer decides a page is ready for
visitors, it is added to that room's allowlist and copied here, and this repository's GitHub Pages site lists it on a
shelf. Until then the shelves say where each piece waits.

```mermaid
flowchart LR
  L["the lab's desks<br/>(drafts)"] -->|"allowlist"| R["reading-room<br/>(private: members read<br/>through the readers team)"]
  R -->|"PUBLIC-ALLOWLIST.txt<br/>both tripwires"| P["reading-room-public<br/>(this repository)"]
  P -->|"GitHub Pages"| S["the shelves at<br/>theholyearthfoundation.github.io/<br/>reading-room-public"]
  V["you"] --> S
  M["members"] -->|"sign in"| R
```

## <img src="assets/icons/sprout.svg" width="24" height="24" alt=""> What is here

| File | Owned by | What it does |
|---|---|---|
| `index.html`, `assets/`, `.nojekyll` | this repository | the front end: one static page in the foundation's amber, no build step, readable on a phone, light and dark |
| `README.md` | this repository | this page |
| `room-manifest.json` | the sync | the list of files the sync copied, read by the front end (absent until the first sync) |
| `proposals/`, `procedures/`, `decks/` | the sync | only the paths an officer has allowlisted: *Start here* and the procedures every organisation in the fleet shares are listed; they arrive on the first sync after the deploy key exists |

## <img src="assets/icons/shield-check.svg" width="24" height="24" alt=""> How it is kept

- **Nobody edits the synced folders by hand.** The private room's sync copies exactly its allowlisted paths after two
  tripwires: the first stops anything that looks like a credential or an internal note; the second reads **every**
  file, PDFs included, and refuses one that no machine could read unless a person attested they read it. A public
  lane never publishes a file a machine or a person has not read (SOP-OPS-003). The front end's own files are never
  overwritten by it.
- `main` cannot be deleted (a deletion-only ruleset). Pages builds from `main`, at the root.
- To change the front end, open a pull request here; to change what is published, change the allowlist in the private room.

## <img src="assets/icons/lock.svg" width="24" height="24" alt=""> Reading the members' room

The members' room is <https://github.com/theholyearthfoundation/reading-room>. Members of the foundation send their
GitHub username (never a password or a code) to the steward or to Kenney, accept the invitation, and read the private
room in a browser. A **404** there means "not yet invited" or "signed out", not "broken". New to GitHub? The
procedure *New to GitHub: your first hour* (SOP-COM-001) walks the whole first hour; the page's *Read the members'
room* section has the short version.

## <img src="assets/icons/link.svg" width="24" height="24" alt=""> Elsewhere

- <img src="assets/icons/globe.svg" width="16" height="16" alt=""> [The foundation →](https://theholyearthfoundation.github.io)
- <img src="assets/icons/presentation.svg" width="16" height="16" alt=""> [Welcome to The Holy Earth Foundation](https://github.com/theholyearthfoundation/.github/blob/main/decks/welcome.marp.pdf), the welcome deck
- <img src="assets/icons/scroll-text.svg" width="16" height="16" alt=""> The procedures' public twin: [`ops-standard-operating-procedures-public`](https://github.com/theholyearthfoundation/ops-standard-operating-procedures-public)
- <img src="assets/icons/book-open.svg" width="16" height="16" alt=""> The lab's public proposals preview: [`drasticstatic/proposals-thef-public-preview`](https://github.com/drasticstatic/proposals-thef-public-preview)
