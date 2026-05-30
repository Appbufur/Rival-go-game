# Rival Go Game

**Real-time multiplayer browser game. No install. No sign-up. Share a link and play.**

[rivalgogame.com](https://rivalgogame.com)

---

## Overview

Rival Go is a browser-based multiplayer game platform built on WebRTC/P2P architecture. It supports 2–10 players per session and runs entirely in the browser with no server-side game logic for match state — connections are peer-to-peer.

The platform currently ships two game modes:

<img width="900" height="864" alt="Launch4" src="https://github.com/user-attachments/assets/c5dea12c-0fba-419a-b013-d13c7315f9bb" />
---

## Game Modes

### Memory

A real-time card matching game. The board is populated with face-down card pairs. Both players flip cards simultaneously — there are no turns. Cards can be of three types: colors, tech/object emojis, or numbers. Grid size is configurable: 5x5, 6x6, 7x7, or 8x8. Match timer options: 60s, 120s, 180s, 300s.

Scoring: a matched pair is awarded to whichever player flips the second card of the pair first. Most matches when the timer expires wins. Real matches award 5 wins to the winner; bot matches award 1.

<img width="365" height="364" alt="Launch" src="https://github.com/user-attachments/assets/3abe9dc3-33d8-4976-9d19-9f66feb1bf3f" />

### Block Merge

A block placement game where players place falling or selectable blocks onto a shared or individual board to clear lines and accumulate score. The objective is to clear the board by merging and eliminating block formations. Designed as a secondary competitive mode alongside Memory.

<img width="914" height="877" alt="Block merge" src="https://github.com/user-attachments/assets/c9e69ff9-7eb8-4d1d-a537-cc3ce8e5c38e" />
---

## Daily Challenges

**Daily Grid** — A fixed Memory board, identical for all players each day. Resets every 24 hours. Completion time is tracked and posted to a global leaderboard. Results are shareable (similar to Wordle score sharing).

**Daily Block Blast** — A daily challenge variant for the Block Merge mode. Same mechanic: fixed daily puzzle, global leaderboard, shareable result.

---

## Technical Notes

- Transport: WebRTC (P2P), no relay server required for matched peers
- Frontend: HTML5 / JavaScript
- No backend required to start or run a match
- Fully responsive — desktop and mobile browsers supported
- Session persistence via localStorage (auto-login)

---

## Features

- 2–10 player lobbies
- Bot support (solo practice, awards reduced wins)
- Global all-time and season leaderboards
- Daily Race leaderboard (time-based)
- Account system with win tracking (optional — guest play available)
- Invite via shareable link or Web Share API

---

## Links

- Website: [rivalgogame.com](https://rivalgogame.com)
- YouTube: [youtube.com/@Rivalgogame]
