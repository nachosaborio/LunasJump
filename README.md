# 🌙 Luna's Jump 🐾

![GameMaker](https://img.shields.io/badge/GameMaker-GML-8A2BE2?logo=gamemaker&logoColor=white)
![Language](https://img.shields.io/badge/language-GML-5C4EE5)
![Platform](https://img.shields.io/badge/platform-HTML5%20%7C%20Android-1f6feb)
![Genre](https://img.shields.io/badge/genre-Platformer-ff69b4)
![Status](https://img.shields.io/badge/status-Released%20v1.0-success)
![Rating](https://img.shields.io/badge/itch.io-%E2%98%85%205.0%2F5-fa5c5c?logo=itchdotio&logoColor=white)
[![Play on itch.io](https://img.shields.io/badge/%E2%96%B6%20Play-itch.io-FA5C5C?logo=itchdotio&logoColor=white)](https://nachodeveloper.itch.io/lunas-jump)

A vertical **infinite-platformer** (Doodle Jump–style) built in **GameMaker (GML)** and released on **itch.io** for **HTML5 and Android**. Made as a fan game for **Luna Rurine**, a vtuber from the (now-defunct) agency **Wactor**.

> ⭐ Rated 5.0/5 on itch.io · Published 2022 · Playable in-browser and as an Android APK.

**▶️ Play it:** https://nachodeveloper.itch.io/lunas-jump

---

## About the game

Luna climbs endlessly upward across procedurally-spawned platforms, dodging enemies and grabbing power-ups themed around the character and her community. Miss a jump or get caught, and it's game over — so chase that high score.

- **Controls:** Arrow keys (⬅️➡️) or tap/click the left/right side of the screen. Full keyboard **and** touch support.
- **Platforms:** three types — normal (white), bouncy (blue), and fragile (red) — with a tuned difficulty curve.
- **Power-ups:** Bepis jetpack, Bubble-tea shield (blocks the next cheese), color-swapping broccoli, Luna Buebo, and bananas as currency.
- **Skins shop:** spend collected bananas on 7+ unlockable Luna skins (hooded Luna, chef Luna, DD Slayer, RuriNewMoon, Tía Pelusa, and more).
- **Extras:** persistent high scores, an interactive tutorial, background music with volume control, screen transitions, a secret ending past 150 points, and two cheat codes (try typing `PUNK` during gameplay 😉).

---

## My role

**Solo developer & project director.**

I programmed the entire game in GML and directed a collaborative production of **8 people** — coordinating art, music, and testing into a single shipped product:

| Role | People |
|---|---|
| 🎮 Development & direction | **NachoDev** (me) |
| 🎨 Art | ブランドン, MelonPan, My Dearest Alice, Andrés |
| 🎵 Music & SFX | GerX, Merol |
| ✔️ Testing | Ben Brightwell, Lomitos |

This was as much an exercise in **leading a small creative team to ship** as it was in programming.

---

## Technical highlights

All game logic is written in **GML** across ~150 object event scripts and a handful of reusable scripts. Some of the more interesting systems:

- **Procedural platform generation** with an infinite vertical scroll and three platform behaviors (`objPlatform`, `objJumpCollision`).
- **Physics-based player** using GameMaker's `speed` / `gravity` / `direction`, with collision handlers for 9 distinct entity types (enemies, platforms, each power-up).
- **Power-up system** — each power-up is its own object with its own behavior (`objBepis`, `objBoba`/shield, `objBrocoli`, `objBuebo`, `objPlatano`).
- **In-game skins shop** (`scrShop`, `objShopTriangle`) — banana currency, index-based skin selection across 7 skins, persisted via `global` state.
- **Save system** for high scores, plus a cheat-code engine (`objCheats`) with a hidden skin.
- **Responsive canvas scaling** (`scrscalecanvas`) so the game adapts to HTML5 and mobile resolutions.
- **Dynamic audio** (`objmusic`) with multiple BGM tracks and a player-controlled volume bar.
- **Screen transitions & fades** (`objTransition`, `oFade`, `fadeToRoom`) between menu, tutorial, game, shop, and credits.

**Engine:** GameMaker · **Language:** GML · **Targets:** HTML5, Android

---

## Development log

The game shipped **v1.0 on 2022-06-19** after ~5 months of iterative development (first prototype 2022-01-25). Highlights from the devlog:

- Infinite platform spawning + three platform types (v0.1a)
- Cheese enemy, Bepis jetpack, touch controls (v0.2a–v0.3a)
- Bubble-tea shield + score saving (v0.4a–v0.5a)
- Full art/music pass: start screen, game-over, BGM, SFX, Luna sprites (v0.6a)
- Banana currency, broccoli power-up, Luna Buebo (v0.7a–v0.10a)
- Skins shop + pause/restart/menu buttons (v0.11a–v0.12a)
- High-score save, credits screen, cheat codes (v0.13a)
- Volume config, clearer font, tutorial, screen transitions, secret ending (v0.14a–v0.17a)
- Luna voice lines + Android APK release (v0.18a–v0.9b)

_(Full version history on the [itch.io page](https://nachodeveloper.itch.io/lunas-jump).)_

---

## Credits & licensing

The **code** in this repository was written by me (NachoDev) and is shared for portfolio and educational purposes.

⚠️ **The art, music, sound effects, and the Luna Rurine character are the property of their respective creators** (credited above) and are **not** covered by any open-source license. They are included here only to make the game buildable and are **not** free to reuse. Please do not reuse the assets without the creators' permission.

---

## Author

**Sergio Ignacio Saborío Segura** — "NachoDev"
Solo developer & director · Informatics Engineer
🎮 itch.io: https://nachodeveloper.itch.io/lunas-jump
