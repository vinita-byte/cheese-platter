# 🧀 Cheese Platter

**Tap "Find My Cheese" for a filmy Bollywood pickup line — and exactly when to use it on a date.**

🔗 **Live:** https://cheese-platter.vercel.app

---

## What it is

Cheese Platter is a one-tap randomiser for cheesy Bollywood pickup lines and filmy dialogues. Every line arrives with a *scenario* — the exact moment on a date where it actually lands — so you get the delivery, not just the dialogue.

100+ lines, built as a small, fast, single-page web toy. No sign-up, no tracking, no build step.

## Features

- 🎲 One-tap randomiser with a poster-style reveal
- 🎬 A "when to use it" scenario attached to every line
- 🔊 Random landing sounds, with mute and volume control
- ✨ Splash screen and an animated spin state
- 📱 Mobile-first layout
- 🔤 Self-hosted fonts — no third-party font requests

## Stack

| Thing | Choice |
| --- | --- |
| Markup, styles, logic | Vanilla HTML, CSS and JavaScript, all in one `index.html` |
| Fonts | Self-hosted in `/fonts` |
| Audio | Self-hosted in `/sounds`, plain `Audio` API |
| Hosting | Vercel |
| Build step | None |

No framework, no bundler, no dependencies.

## Run it locally

```bash
git clone https://github.com/vinita-byte/cheese-platter.git
cd cheese-platter
python3 -m http.server 8000
```

Then open `http://localhost:8000`.

Opening `index.html` straight from the filesystem mostly works, but serving it over HTTP keeps the font and audio paths behaving.

## Project structure

```
index.html     # the whole app — markup, styles, lines and logic
fonts/         # self-hosted webfonts
sounds/        # landing sounds
favicon.svg    # and the other icons
```

## Credits

Made by [Vinita Mathreja](https://github.com/vinita-byte) — more at [WhatTheWeb](https://whattheweb.co.in).

The lines are affectionate parodies of Bollywood tropes. Any dialogue references belong to their original films and writers.
