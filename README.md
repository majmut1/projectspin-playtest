# Project Spin — Beta 1 playtest build

A hosted build of an in-development game, published so the owner can open it on a
phone. **This repository holds no source code** — only the compiled Web export.

**▶ Play: <https://majmut1.github.io/projectspin-playtest/>**

---

## What it is

Arcade table tennis. One local match against a bot: first to 7, no win-by-two.

| | |
|---|---|
| **Move the bat** | Drag anywhere on the screen, or move the mouse. The bat moves *with* your finger — it does not jump to it. |
| **Serve** | **Flick upward.** Wait ten seconds and the game serves for you. |
| **Aim** | Where the ball meets the bat decides where it lands. Low on the bat sends it deep, high sends it short, off to one side sends it that way. |
| **⚠️ If the ball is going out, let it go** | Hitting it before it bounces on your side loses you a point that was already yours. |

## Build

Godot 4.7.1, `Web NoThreads` preset. The non-threaded variant is used because
GitHub Pages cannot send `Cross-Origin-Opener-Policy` / `Cross-Origin-Embedder-Policy`,
which a threaded build needs for `SharedArrayBuffer`. The game itself is identical
— the `.pck` is byte-for-byte the same as the threaded build.

Development happens in a separate private repository. This one is regenerated
from it and carries no history worth reading.
