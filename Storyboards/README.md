# REVENANT SLEUTH — Storyboard System
**How to Use These Files in Unreal Engine and Blender**

---

## Numbering Scheme

Each storyboard file is named using the following format:

```
SB_S{season}E{episode}_Sc{scene} — Scene Title.md
```

**Examples:**
- `SB_S01E01_Sc01 — December Briefing.md` → Season 1, Episode 1, Scene 1
- `SB_S02E04_Sc02 — The Diner Witness.md` → Season 2, Episode 4, Scene 2
- `SB_S03E01_Sc01 — The First Name.md` → Season 3, Episode 1, Scene 1 (PROJECTED)

**Season range:** S01–S05
**Episode range:** E01–E06 (varies by season; see Production/Series-Bible.md)
**Scene range:** Sc01–ScXX (as many scenes as the episode contains)

---

## Folder Structure

```
Storyboards/
├── Season-01/
│   ├── Episode-01/   → S01E01 scenes (Ch.1a–d)
│   ├── Episode-02/   → S01E02 scenes (Ch.1e–g)
│   ├── Episode-03/   → S01E03 scenes (Ch.2 all)
│   ├── Episode-04/   → S01E04 scenes (Ch.3a–c)
│   ├── Episode-05/   → S01E05 scenes (Ch.3d–e)
│   └── Episode-06/   → S01E06 scenes (Ch.4a–c)
├── Season-02/
│   ├── Episode-01/   → S02E01 scenes (Ch.4d–f)
│   ├── Episode-02/   → S02E02 scenes (Ch.4g–h)
│   ├── Episode-03/   → S02E03 scenes (Ch.5a–b)
│   ├── Episode-04/   → S02E04 scenes (Ch.5c–d)
│   ├── Episode-05/   → S02E05 scenes (Ch.5e–f)
│   └── Episode-06/   → S02E06 scenes (Ch.6 — DRAFT)
├── Season-03/        → PROJECTED (Ch.7–8 outline boards)
├── Season-04/        → PROJECTED (Ch.9–10 outline boards)
└── Season-05/        → PROJECTED (Ch.11 + epilogue outline boards)
```

---

## Status Labels

Every storyboard file is labeled in its header:

| Label | Meaning |
|---|---|
| *(no label)* | Fully sourced from The Story; canon |
| `DRAFT` | Sourced from Ch.6 rough draft; subject to revision when Ch.6 is finalized |
| `PROJECTED / OUTLINE` | Built from Character Bible extrapolation; beat-level only; not source-of-truth |

---

## Storyboard Template

Every storyboard file uses this exact template:

```markdown
# SB_S0XE0Y_ScZZ — <Scene Title>
- Source: <The Story chapter/section, or "PROJECTED from Character Bible">
- Location: INT./EXT. <place> — <time of day / weather>
- Characters: <list>
- Beat summary: <2–4 sentences of what happens and why it matters>

## Shot List
| # | Shot | Framing/Move | Subject | Notes (lighting, lens, VFX) |
|---|------|--------------|---------|------------------------------|

## Blocking & Camera
<staging, movement, eyelines, mirror usage if relevant>

## Dialogue (adapted — consistent, not exact)
<short lines; may compress/adjust the book for pacing while preserving meaning and noir voice>

## Lighting & Color
<palette + key/fill/practical sources>

## Audio / Bass Cue
<score, diegetic music, and any "command/bass" signature beats>

## Low-Poly Asset Notes
<environments/props/characters to model or reuse>

## Continuity Flags
<callbacks, foreshadow-only signatures, reveal-discipline reminders>
```

---

## How to Use in Unreal Engine

1. **Scene setup:** Each storyboard file corresponds to one Unreal level sequence or sequencer cut. The `Location` field tells you which environment asset to load (cross-reference `Production/Asset-List.md`).
2. **Shot list → Sequencer cameras:** Each numbered shot in the Shot List becomes one camera cut in the Level Sequencer. The Framing/Move column describes the camera type (static, dolly-in, track-left, etc.).
3. **Characters:** The Characters field tells you which character meshes to place in the scene.
4. **Audio:** The `Audio / Bass Cue` field tells you which audio assets to drop into the sequence (cross-reference `Production/Asset-List.md` — Audio section A01–A07).
5. **VFX:** The `Notes` column in the Shot List calls out VFX system requirements (cross-reference `World/Props-and-Motifs.md` and `Production/Asset-List.md` — VFX section).

## How to Use in Blender

1. Each storyboard file = one Blender scene or one collection within a master .blend file.
2. Import characters as linked libraries from a master character .blend file — this keeps updates synchronized.
3. The `Low-Poly Asset Notes` section calls out which assets can be reused from existing builds vs. which need new geometry.
4. Camera blocking notes translate directly to Blender camera objects in the scene. Set up each shot as a keyframe on the camera with the described movement.

---

## Reveal Discipline Reminder (All Boards)

> **The Lich Lord truth is NEVER explicit before Chapter 10–11 material.**
> Any storyboard, caption, or adapted dialogue that makes the Lich's nature explicit before Season 4 Episode 5 (at earliest) must be revised.
> 
> Foreshadow freely: cold, bass, stitching, mirrors, archaic language.
> Explain nothing.

---

## Adapted Dialogue Rule (All Boards)

> Dialogue in storyboards is adapted — **consistent with the source, not exact.**
> Lines may be compressed, reordered, or paraphrased for visual pacing.
> They must preserve meaning, voice, and any K-flag content.
> Read each adapted line aloud. If it could not plausibly have been written by the same person who wrote:
> *"I watch. I listen. I bury what I can't fix."*
> — revise it.
