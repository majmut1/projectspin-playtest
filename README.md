# CROWN//BREAK — vertical slice

A hosted build of an in-development game, published so the owner can open it on
a phone. **This repository holds no source code** — only the compiled Web export.

**▶ Play: <https://majmut1.github.io/projectspin-playtest/>**

---

## What it is

A 4-player kinetic possession brawler for portrait mobile. You plus three bots.

| | |
|---|---|
| **Move** | Drag anywhere. The body steers toward your finger — there is no on-screen stick. |
| **Dash** | **Flick** fast in a direction. A dash commits: miss and you are briefly helpless. |
| **Take the Crown** | Touch it. Holding it fills your meter — the ring closing around the arena floor. |
| **Break the holder** | Dash into them at speed. The Crown pops loose and everyone scrambles. |
| **Counter** | Dash as an attacker commits and you deflect them instead. |

First to 20 cumulative seconds of possession wins.

## Build

Godot 4.7.1, `Web NoThreads` preset. The non-threaded variant is used because
GitHub Pages cannot send `Cross-Origin-Opener-Policy` / `Cross-Origin-Embedder-Policy`,
which a threaded build needs for `SharedArrayBuffer`.

Development happens in a separate private repository. The previous project,
Project Spin, is preserved on the `archive/project-spin` branch of both
repositories.
