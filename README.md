# AI PROMPT STUDIO — Cinematic Continuity Engine

A Thai-first workspace for planning AI-generated films as linked 10-second clips.

## Product goals

- **Character DNA:** detailed character identity, appearance, wardrobe, voice, props, reference-image notes, and immutable identity fields.
- **Location DNA:** persistent locations with architecture, layout, set dressing, lighting, time, weather, and reference-image notes.
- **Story Continuity Engine:** story bible, multi-genre planning, episode/scene/clip structure, and previous-clip state handoff.
- **Clip Director:** each generated video prompt targets exactly 10 seconds, with shot timing, blocking, natural performance, eye-lines, dialogue, and camera coverage.
- **Dialogue Editor:** edit speaker, exact Thai dialogue, pronunciation notes, emotion, delivery, and performance direction before generating prompts.
- **Continuity Checker:** compare each clip against character, location, prop, wardrobe, and story-state locks.
- **Project Library:** save, reopen, duplicate, export, and import projects.

## Genre choices

Fantasy, wuxia, xianxia, romance, drama, comedy, horror, mystery, adventure, action, revenge, period, slice of life, sci-fi, investigation, thriller, system-assisted, transmigration, multi-genre, and AI-selected supporting genres.

Special mechanics: levels, missions/quests, status windows, system shops, gacha, time regression, reincarnation, world crossing, parallel worlds, and special dimensions.

## Current implementation scope

The first milestone is a usable browser-based MVP with project editing, multi-select genres, Character DNA, Location DNA, Story/Clip planning, editable dialogue, prompt assembly, and local autosave/export/import. Cloud sync and direct video-generation integrations require separate service credentials and will be added only when configured.

## Run locally

```bash
npm install
npm run dev
```

## Stack

- React + TypeScript + Vite
- Browser local storage for MVP autosave
- JSON project export/import for portability

## Product constraints

- One output clip = 10 seconds.
- A clip may contain multiple shots whose durations add up to 10 seconds.
- Keep dialogue short enough to fit the selected clip.
- Never silently modify locked character/location details or approved dialogue.
- Every next clip should inherit the previous clip's ending state.
