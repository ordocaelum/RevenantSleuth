# REVENANT SLEUTH — Characters Visual Reference
**Low-Poly Character Build Guide for Unreal Engine / Blender**
*Silhouette, palette, distinguishing features, and supernatural tells. These are production targets, not photorealistic goals. Readable from 10+ feet on a YouTube thumbnail.*

---

## Core Design Philosophy
Low-poly noir characters succeed by **silhouette and palette**, not detail. Every character should be identifiable at a glance by outline and color. Faces are kept minimal — the expression is in posture, the story is in lighting. Supernatural tells are achieved through material/shader differences, not high-poly sculpting.

---

## 1. Detective ADRIAN KANE — Protagonist

### Silhouette Target
A worn overcoat, slightly too large (inherited or bought when he weighed more). Wide shoulders, but the weight sits lower now — tension below the sternum, not above it. He moves with economy. No wasted motion.

### Base Palette
- **Coat:** Dark charcoal grey, nearly black, with subtle texture variation from years of city use.
- **Suit beneath:** Navy blue, darker than the coat but same family.
- **Shirt:** White that has been washed too many times — off-white. No tie, or tie loosened at the collar.
- **Boots:** Dark brown leather, resoled at some point.
- **Skin:** Medium-warm tone. No idealization.
- **Hair:** Dark, short, slightly overgrown at the sides — the cut of a man who has appointments but doesn't keep them.

### Distinguishing Features (Readable at Low-Poly)
- The coat: **its silhouette is his signature**. Wide lapels, slightly flared below the waist, collar turned up in cold scenes. The coat should be slightly asymmetrical as worn — never sitting perfectly.
- **Bandage on left forearm** (Ch.5 onward): visible below rolled sleeve. White tape over dark bruising; the skin immediately around it is slightly paler than the rest. This is a running visual flag.
- **Hands:** Always doing something. Weapon check, sleeve roll, tapping a surface. In stillness, they look wrong.
- **Eyes:** Low-brow set, heavy. He doesn't look tired — he looks *present*, which is more threatening.

### Supernatural Tell (Ch.5 onward — Bite Progression)
- The bandaged arm: a faint branching pattern just visible at the bandage edge. Dark, like ink under paper. Never dramatic. Just there.
- In cold environments or near the vial: the bandaged area should show a **slight blue-cold tint** in the diffuse material — as if the cold is concentrated there.
- As the series progresses (Ch.7+), the branching pattern can spread slightly further from the wound site. Very subtle. The viewer should notice it before Kane does.

### Animation / Posture Notes
- **Anger = smaller movements.** He doesn't raise his voice or swing wide. He gets quiet and precise.
- **Exits first, then faces.** Every time Kane enters a room, his first glance is toward the exits. This is a low-poly animation note: have the character head-track toward exits (2–3 beat delay) before settling focus.
- **The sleeve roll:** a repeated physical tell. Any scene where Kane is preparing for action, he rolls one sleeve.

### Low-Poly Build Target
- Poly count: 800–1200 tris for the character mesh
- Key shapes: broad coat shoulders, slight forward lean, boots with slight heel lift
- Texture: single 512×512 atlas with body + face + coat
- No face normal map needed — flat-shaded with baked shadows is the correct noir aesthetic

---

## 2. Evelyn SINCLAIR — Deuteragonist / Partner

### Silhouette Target
Elegant steel. She doesn't fill space — she controls it. Her silhouette is more contained than Kane's, more deliberate. Where Kane's coat is a wound flag, Evelyn's coat is **armor**.

### Base Palette
- **Coat (Ch.1–4):** Dark burgundy-red, well-cut, structured. She wears clothes that communicate she belongs wherever she is.
- **Coat (Ch.5+):** Shifts to darker navy or dark slate — less warm, more operational. The wardrobe shift mirrors the POV naming shift.
- **Beneath:** Black trousers, structured blouse (grey or white). Clean lines.
- **Shoes:** Low heels or flat boots — she needs to move, but she needs to look like she doesn't need to.
- **Hair:** Dark, pulled back — not tightly (that would be severity); simply, efficiently.
- **Skin:** Warm medium, slightly paler than Kane. In Ch.5+ scenes, slightly more pallor — the bass exposure taking its toll at the subconscious level.

### Distinguishing Features
- **Posture:** Completely composed even when hurt. Her spine doesn't curve. She doesn't hunch. This is her tell — stillness under duress.
- **Eye contact:** She holds it longer than is comfortable. A low-poly character can communicate this via sustained head-lock toward whoever she's speaking with, not tracking away.
- **Bruise (Ch.5):** Visible along cheekbone — purple-to-yellow gradient on the diffuse texture. Blood dried at the corner of her mouth, cleaned by mid-Ch.5.
- **Comms earpiece (Ch.3–4):** Small in-ear device, hidden under hair on one side.

### Supernatural Tell (Ch.4 onward — Bass Sensitivity)
- In scenes where the bass/rhythm command is present: **a subtle shoulder tension** — not a flinch, but the posture equivalent of bracing. Her hands close slightly. Her jaw sets.
- In Ch.6+: when the bass command is strong enough, she shows a slight postural *pull* — her body turning fractionally toward the source before she catches herself and corrects.
- This is depicted via animation/posture only. No visual distortion on her model.

### Low-Poly Build Target
- Poly count: 800–1200 tris
- Key shapes: structured coat (no flare, clean cut), straight spine, slight heel in boots
- Texture: single 512×512 atlas
- Ch.5 version: same mesh, variant texture with bruise on cheekbone

---

## 3. MAX — Primary Human Antagonist

### Silhouette Target
Max is what Kane could have become. That's the point. The silhouette is *similar* — same detective build, same era, similar coat. But something has rotted in the posture. He stands too still. He turns too slowly. He looks like a man practicing at being human.

### Base Palette
- **Coat:** Dark grey-green — the same charcoal family as Kane's but with a military, almost uniform quality. Longer, straighter cut. Deliberate.
- **Beneath:** Dark suit, white shirt — but the shirt collar is never quite right. Off by one button. Something that's close to put-together but not.
- **Hands:** Pale. Not supernaturally pale — but compared to the rest of him, the hands look like they belong to someone older.
- **Hair:** Dark, cut precisely. Too precisely — like a man who wants to communicate he controls himself completely.

### Distinguishing Features
- **The pause:** Max stops mid-sentence and looks slightly away, as if listening to something no one else hears. This happens once per scene, minimum. It should feel odd from the first time you see it. Low-poly animation: head drifts 5–10 degrees away from conversational partner during pause; returns on the next spoken word.
- **Archaic diction flag (visual):** In close-up adapted dialogue, certain words ("tribute," "fealty," "court") should be delivered with a slightly different cadence — slower, with more weight — as if he's quoting something.
- **Eye contact:** Very direct, very deliberate. He uses Kane's name when he makes it. If he ever says "Adrian," it should feel like a key turning in a lock.

### Supernatural Tell (Escalates Through Ch.7–11)
- **Ch.7–8 (projected):** Slightly longer pauses. Slightly more archaic vocabulary.
- **Ch.9–10 (projected):** Branching vein pattern faintly visible at the jaw/temple — the same ink-under-paper look as the homeless man in Ch.2. Still deniable. Still foreshadow-only.
- **Ch.11 (projected):** When partially "claimed," the cold is visible in him — a slight blue-grey tint in his skin diffuse, the branching veins now prominent, his breath fogging in warm rooms.

### Low-Poly Build Target
- Poly count: 800–1200 tris (same as Kane — they should look like mirror images at a glance)
- Key shapes: longer coat, slightly more rigid posture (less organic movement in cloth simulation)
- Texture: include subtle jaw/temple vein overlay that can be composited more prominently in later seasons

---

## 4. VOSS — Secondary Antagonist

### Silhouette Target
The frontman. He's not imposing through size — he's imposing through theatricality. His silhouette reads as *designed*. He dresses like a man who has decided what performance looks like.

### Base Palette
- **Primary:** Deep violet-black suit (echoes the club's neon). Well-tailored. The kind of suit that says someone spent money.
- **Shirt:** Burgundy or dark red, no tie. Collar open just enough to seem relaxed, which makes it more deliberate.
- **Accessories:** A ring (one, heavy-set). Shoes that are too polished for the environment.
- **Skin:** Pale but not supernaturally — the pale of someone who hasn't been outside in years.
- **Hair:** Dark, swept back. Controlled.

### Distinguishing Features
- **The ring:** Used in blocking — he turns it when frustrated, taps it when impatient. A low-poly character can sell this with a single wrist-rotate animation.
- **The voice:** (For VO casting) — smooth, amused, slightly affected. When his control is threatened, the amusement thins but never disappears. Anger as restraint.
- **Height:** Taller than Kane by a few inches. This should be readable in silhouette — it gives him visual dominance in shared shots until Kane closes distance.

### Supernatural Tell
- Voss doesn't have a visible supernatural tell (he's a node in the system, not a user).
- The *tell for the audience* is behavioral: he stops mid-action when the Lich overrides him. He started to give an order and then simply... didn't. This should look like a freeze-frame, a half-second of vacancy, before he continues on a different course.

---

## 5. THE LICH LORD (Indirect Presence Only — No Direct Model Until Ch.11)

### Before the Reveal
The Lich Lord is never shown directly before Ch.10–11. What the audience sees:
- **The shape in the mirror:** A dark, hunched silhouette in the Ch.4 basement mirror. Human-adjacent but wrong — too long in some proportion, too still. This is a simple low-poly silhouette model, rendered only in the mirror layer.
- **The figure in the fog (Ch.6):** The dark-coated watcher at the dock. This can be the same silhouette model as the mirror shape, at much greater distance, obscured by fog.

### Reveal Model (Ch.11 — Projected)
At the full reveal, the Lich Lord should be:
- **Ancient, aristocratic, wrong.** Not monster-large — imperial-still. The horror is not scale but *patience*.
- **Pale as void** — not white but the absence of warmth in skin.
- **Robes or heavy vestments** — archaic, formal, the "court" aesthetic made literal. Dark material with the sigil/marking pattern incorporated into the fabric.
- **Cold visible around it** — the breath-fog effect, but generated by the Lich's proximity rather than the environment.

---

## 6. Lt. MARISOL GRANT

### Silhouette Target
Authority-dressed-practically. Grant isn't theatrical. She is the institution given a face.

### Base Palette
- **Professional suit/blazer:** Dark navy or charcoal. The cut is functional, not fashionable.
- **Shirt:** White or light grey. Collar buttoned.
- **Reading glasses (often in hand):** Small, rectangular frames.

### Distinguishing Features
- **Eyes sharp enough to cut paper** (per the prose).
- **The coffee cup** — she is never without it, never surprised without it. It's a prop that signals she is always working.
- **Seated posture:** Leaned slightly forward, not relaxed. She doesn't own a relaxed mode.

---

## 7. Dr. HARLAN CHO

### Silhouette Target
A man who keeps his hands steady through discipline. The coroner as moral anchor — the most rational person in the room, being slowly eroded by the irrational.

### Base Palette
- **Lab coat (work scenes):** White, clean, with pen in breast pocket. This is his armor.
- **Personal (late-night Ch.6 scene):** Shirtsleeves and suspenders. Tie loosened. This is the first time we see him without his armor. It makes the Ch.6 morgue scene more frightening.
- **Glasses:** Worn for close work; removed when thinking. The glasses-removal is a tell.
- **Age:** Late 40s–50s. Silver at the temples.

### Supernatural Tell
- No physical contamination — Cho never touches essence directly (gloves always).
- His tell is behavioral: the test he runs for the fourth time. The temperature probe he checks twice. The note he writes to himself: "DO NOT BE ALONE WITH IT TOO LONG." The frightening thing about Cho is that he's *trying* to be rational and the rational instruments are failing.

---

## 8. Officer "ROOK" ALVAREZ

### Silhouette Target
Young. Present. The one who still believes backup always comes — until he doesn't. A human mirror for the rookie in the body-cam footage.

### Base Palette
- **Uniform:** Standard patrol blues. Precinct standard.
- **No detective affectations** yet — this is part of his characterization. He looks exactly like what he is.
- **Build:** Lean, upright. The posture of someone who still cares about the impression he makes.

### Distinguishing Features
- **Youth:** His face is the youngest in the cast. This should be readable in low-poly — slightly softer geometry (less jaw, less brow weight).
- **The tell that makes him narratively dangerous:** When near bass-heavy environments or contaminated persons, he *almost* stops — a brief flicker of the same compliance the users show. But he catches himself. It's barely visible. It means he's already been exposed at some level.

---

## General Low-Poly Character Notes

### Shared Build Standards
| Character | Poly Count | Texture Atlas | Shadow Pass |
|---|---|---|---|
| Kane | ~1000 tris | 512×512 | 2-tone baked |
| Sinclair | ~1000 tris | 512×512 | 2-tone baked |
| Max | ~1000 tris | 512×512 (mirror of Kane) | 2-tone baked |
| Voss | ~900 tris | 512×512 | 2-tone baked |
| Grant | ~700 tris | 512×512 | Flat |
| Cho | ~700 tris | 512×512 | Flat |
| Rook | ~700 tris | 512×512 | Flat |
| Mirror-shape (Lich shadow) | ~200 tris | 128×128 (silhouette) | Pure shadow |

### Consistent Cross-Character Rules
1. **Faces are never the focus.** Lighting, posture, and palette carry emotion. Face geometry should be minimal (flat-plane with texture, baked highlight).
2. **Hands are always modeled** (not mittens). The hands matter — Kane's hands are a recurring tell.
3. **Breath particle** on all characters in exterior December scenes. Single-emitter, very low particle count (3–5 puffs per breath cycle). It is the cheapest way to communicate "this world is cold and real."
4. **The supernatural tells are material/shader differences**, not geometry. Adding a blue-cold tint to an arm's texture is free. Adding geometry for branching veins is expensive.
