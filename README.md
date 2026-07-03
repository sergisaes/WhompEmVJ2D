<h1 align="center">Whomp'Em — 2D Platformer</h1>

<p align="center">
  A side-scrolling 2D action platformer written from scratch in C++ and OpenGL —
  tile levels, moving platforms, enemies, bosses, power-ups and a HUD, with FMOD audio.
</p>

---

## What it is

A complete 2D platformer game engine and game, built for the Video Games (VJ) course. No game
engine — the rendering (OpenGL + GLSL shaders), sprite animation, tile maps, collision, audio
and game loop are all hand-written in C++.

## Features

- **Player** with animated states, jumping, combat and power-ups.
- **Enemies & bosses** — patrolling enemies (`Orco`), a boss fight (`Boss`), hazards (`FallingStick`).
- **Level system** — tile maps loaded from text files, with foreground / collision / platform layers.
- **Moving platforms**, power-ups, and a HUD tracking health and score.
- **Audio** — music and SFX via FMOD (`AudioManager`).
- **Rendering** — OpenGL with custom GLSL shaders and a sprite/keyframe animation system.

## Architecture

```
Game            → main loop, input, state
Scene           → tile map, entities, camera
Player / Boss / Orco / FallingStick   → entity logic
MovingPlatform / PowerUp / HUD        → world objects & UI
Shader / ShaderProgram / AnimKeyframes → rendering & animation
AudioManager    → FMOD music + SFX
```

## Build

Windows / Visual Studio project under `Projecte/2DGame/WhompEm/`. Requires OpenGL, GLEW, FreeType
and FMOD (bundled). Open the solution and build the `WhompEm` project.

## Stack

C++ · OpenGL · GLSL · GLEW · FreeType · FMOD
