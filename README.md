# 50 States Quest 🗺️

A gamified, self-contained web app for learning all fifty U.S. states — built so every kind of learner has a way in.

**Live demo:** https://claude.ai/code/artifact/42088d61-0d1b-489e-a9ef-a391b5b34b0e

## Five ways to learn

| Mode | Learning style | What you do |
| --- | --- | --- |
| 📅 **Daily Challenge** | Habit · Streaks | Five questions a day, the same for everyone (seeded by the date). Play every day to grow your streak. |
| 🗺️ **Map Room** | Visual · Kinesthetic | Three sub-modes on a real US map: **Explore** (field-guide cards), **Find It** (a name flashes, you locate it), and **Borders** (tap every state that neighbours the target). |
| ✍️ **Quiz Arena** | Test · Compete | 10-question rounds on capitals, nicknames, regions, and state *shapes* — plus **Beat the Clock**, a 60-second rapid-fire run. |
| 🃏 **Flashcards** | Visual · Reading | Flip through shape, capital, nickname, and a memorable fact for all 50. Filter by region, mark what you know. |
| 🎵 **Rhyme Radio** | Auditory | Five regional rhymes read aloud (browser text-to-speech) so the states stick like a song lyric. |
| 🏅 **Badges** | Motivation | Twelve unlockable badges tracking streaks, states located, capitals mastered, speed runs, daily streaks, and more. |

**Capital jingles** — every state–capital pair has a short mnemonic (e.g. *"You-tah shakes the salt in Salt Lake City"*) shown on flashcards, in the map's field-guide card, and after capital quiz questions, with a 🔊 tap-to-hear button.

Points, streaks, badges, best runs, and daily streaks all save automatically in the browser (via `localStorage`).

## Running it

It's a single file with no build step or dependencies. Just open it:

```bash
open index.html      # macOS
# or double-click index.html, or serve it:
python3 -m http.server
```

Works offline once loaded. Light/dark themes follow your system and can be toggled; narration (🔊) can be turned on/off.

## How it's built

- **One file, no dependencies** — HTML, CSS, and vanilla JavaScript inlined in `index.html`.
- **Design** — a "field-guide / national-park atlas" identity: pine-green + sunset-amber on a mist/deep-pine ground, serif display type, and monospace used for postal codes and stats.
- **State geometry** — the interactive map uses shapes from the open-source [`@svg-maps/usa`](https://www.npmjs.com/package/@svg-maps/usa) package (CC BY-NC 4.0).
- **Accessibility** — keyboard-navigable map, focus states, reduced-motion support, and every rhyme is readable as text even without audio.

## Content

All 50 states include capital, nickname, region, and a fun fact. Washington, D.C. appears on the map as a bonus (and is clearly marked *not a state*). The five regional rhymes together cover all 50 states exactly once.
