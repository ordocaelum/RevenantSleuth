# REVENANT SLEUTH — Master Asset List
**Low-Poly Asset Checklist for Unreal Engine / Blender**
*Reused assets are noted once and marked (REUSE) at subsequent references.*
*Priority: Season 1–2 production assets are marked [P1]. Season 3–5 / projected assets are marked [P2].*

---

## ENVIRONMENTS

### E01 — City Street (Wet, Night, December) [P1]
- **Use:** Multiple exterior scenes throughout all seasons
- **Key elements:**
  - [ ] Wet asphalt plane (reflection shader, animated neon overlay)
  - [ ] Sidewalk plane (variation texture)
  - [ ] Street lamp pole + sodium bulb (amber point light, cone shadow cast)
  - [ ] Generic building facades (box geometry, 3–4 variants: brick, panel, glass-dark)
  - [ ] Fog layer (low-lying plane, near-transparent, animated slow drift)
  - [ ] City-glow skybox (near-black blue with far-distance warm haze)
  - [ ] Breath particle system — single emitter, cold blue-white (shared by all characters in outdoor scenes)
- **Notes:** This environment is assembled from reusable modular pieces. Each exterior scene adds location-specific props on top of this base kit.

---

### E02 — The Velvet Abyss, Exterior [P1]
- **Use:** S01E01–S01E02 (Ch.1), S01E04–S01E05 (Ch.3), S01E06–S02E02 (Ch.4)
- **Key elements:**
  - [ ] Club facade (brick + black panel overlay, 3–4 story flat geometry)
  - [ ] Neon sign above entrance (tube-mesh geometry, purple emissive + red accent)
  - [ ] Entrance door (dark wood + amber-gold interior bleed)
  - [ ] Security camera (small geometry, wall-mounted)
  - [ ] Patron queue (crowd billboard sprites, silhouette-level)
  - [ ] Two bouncer positions (flanking entrance)
  - [ ] Adjacent building (generic — for rooftop access scenes)
  - [ ] Fire escape (rusted metal geometry, adjacent building face)
- **Reuses:** E01 base kit

---

### E03 — The Velvet Abyss, Main Floor Interior [P1]
- **Use:** S01E02 (Kane approaches DeMarco), S01E04–S01E05 (Evelyn infiltration)
- **Key elements:**
  - [ ] Long bar (dark lacquer flat-plane counter + stool cylinders)
  - [ ] Bar backlit bottle shelf (amber emissive behind bottle silhouettes)
  - [ ] Dance floor crowd (billboard sprite sheet, animated 12fps)
  - [ ] Speaker stacks (black box primitives, 4 corners)
  - [ ] Booth row (box seats, red UV-mapped upholstery, gold edge material)
  - [ ] Pillar surfaces (box primitives with markings texture overlay — see P01)
  - [ ] Strobe light system (white point lights, animated pulse cycle)
  - [ ] Purple overhead wash (large area light, purple)
  - [ ] Haze layer (slow sprite plane drift, semi-transparent)

---

### E04 — Red Velvet Corridor [P1]
- **Use:** S01E06, S02E01 (the descent into the club)
- **Key elements:**
  - [ ] Tunnel geometry (simple box corridor, ~20m length)
  - [ ] Red wall material (deep red matte with specular at eye level)
  - [ ] Gold trim material (emissive warm gold, applied to wall panel edges)
  - [ ] Sconce lights (simple bracket geometry, amber point light, one per 8 feet)
  - [ ] Double doors at end (heavy dark geometry, gold engraving as normal map)
  - [ ] Markings texture on wall panels (see P01 — same tileable UV)
- **Notes:** The lighting between sconces should be total shadow. The sconce pools are the only lights.

---

### E05 — Basement Factory [P1]
- **Use:** S02E01 (primary), recurring in projected later seasons
- **Key elements:**
  - [ ] Concrete floor (flat plane, stained/drained texture)
  - [ ] Drains (circular decal on floor, no raised geometry)
  - [ ] Metal examination tables x4 (flat box + high-specular metallic material + restraint cylinders on edges)
  - [ ] Industrial overhead fluorescents (flat cool white lights, 2 tubes above each table)
  - [ ] Bound user figures x3–4 (very low-poly, slack-postured, subtle sway animation loop)
  - [ ] Industrial fridge unit (box primitive, keypad decal, cold-blue emissive at door seal)
  - [ ] Vial rows in fridge (instanced P02 vial mesh, visible through cracked-open door)
  - [ ] Side tool table (box, ambiguous clinical props as decal)
  - [ ] Markings on walls (see P01, smaller scale)

---

### E06 — Red-Lamp Side Room [P1]
- **Use:** S02E01 (finding Evelyn), S02E02 (mirror scene)
- **Key elements:**
  - [ ] Small room geometry (box, 4m × 5m, low ceiling)
  - [ ] Red practical lamp (wall bracket + deep red point light, short falloff)
  - [ ] The Black-Framed Mirror (CRITICAL ASSET — see P03)
  - [ ] Armchair (simple box geometry, red upholstery material)
  - [ ] Side table + glass of water (flat-plane table, cylinder glass)

---

### E07 — Rooftop (Adjacent to Club) [P1]
- **Use:** S01E04–S01E05, S01E06 (Kane's observation position)
- **Key elements:**
  - [ ] Flat rooftop plane with rooftop parapet (low-poly brick lip)
  - [ ] Rooftop detritus (HVAC box primitive, pipe cylinder — 2–3 pieces)
  - [ ] Rain system (particle emitter, directional, low count, very small particles)
  - [ ] View toward club entrance across street (requires E02 exterior visible at distance)

---

### E08 — Kane's Apartment Interior [P1]
- **Use:** S01E02 (discovery), S02E03 (crime scene), S02E06 (case box), recurring
- **Key elements:**
  - [ ] Living room/office combo (flat floor plane, 4 walls, ceiling)
  - [ ] Desk (flat box + lamp) with case box on shelf above (cardboard box geometry, label decal)
  - [ ] Chair (simple box geometry — THE crime scene chair)
  - [ ] Rug (flat plane with stain texture overlay — post crime scene)
  - [ ] Shelving unit (box geometry, books as colored box row)
  - [ ] Window (dark, city glow ambient through curtains)
  - [ ] Flashlight VFX (moving spotlight cone, white hard light — used in Ch.1 discovery)
  - [ ] Evidence markers (yellow triangular prisms — post crime scene only)
  - [ ] Yellow tape (line geometry / decal — exterior use)

---

### E09 — Kane's Apartment Building, Hallway [P1]
- **Use:** S01E02 (arrival), S02E03 (arrival)
- **Key elements:**
  - [ ] Corridor box geometry (low ceiling, old carpet texture)
  - [ ] Flickering hallway light (animated emissive — 80% cycle)
  - [ ] Apartment door (flat plane, lock hardware decal)

---

### E10 — Kane's Apartment Exterior / Street [P1]
- **Reuses:** E01 base kit
- **Key elements:** Yellow tape, patrol car (simple box vehicle), two uniform officers (generic low-poly figures)

---

### E11 — The Jazz Bar Interior [P1]
- **Use:** S01E03 (Ch.2 — Kane meets Evelyn)
- **Key elements:**
  - [ ] Single amber bulb above door (exterior practical, warm point light)
  - [ ] Bar counter (dark wood flat-plane + 2 stools)
  - [ ] Bar mirror behind bottles (simple flat-plane with reflection, undecorated)
  - [ ] Bottle shelf (box, amber backlit bottles as emissive)
  - [ ] Jazz musician figure (very low-poly, silhouette + instrument shape — far background)
  - [ ] 2–3 patron shapes (simple silhouettes in shadow booths)
  - [ ] Smoke haze (slow sprite-plane drift, sparse)

---

### E12 — The Motel Room [P1]
- **Use:** S02E03 (Ch.5 opening)
- **Key elements:**
  - [ ] Room box geometry
  - [ ] Nightstand (box) + yellow-shade lamp (emissive warm yellow, full room tint)
  - [ ] Bed x2 (flat rectangular planes + pillow geometry)
  - [ ] Partially-open curtains (flat plane with gap — parking lot sodium bleed through gap)
  - [ ] Bathroom door (ajar, white tile light from within)
  - [ ] TV (box, faint screen glow — diegetic)

---

### E13 — The Morgue / Autopsy Suite [P1]
- **Use:** S02E04 (Cho + vial test), S02E06 (Ch.6 prologue), recurring
- **Key elements:**
  - [ ] White tile walls + floor (flat-plane geometry, high-specular tile material)
  - [ ] Autopsy table (stainless steel box, central, drain below)
  - [ ] Overhead fluorescents (flat cool white — even, no shadows)
  - [ ] Side counter (box) with lab equipment (see props section)
  - [ ] Cho's desk (corner, flat box, legal pad + mug + charm)
  - [ ] Cho's personal fridge (small box unit, keypad, cold-blue emissive seal)

---

### E14 — The Diner [P1]
- **Use:** S02E04 (Ch.5 witness scene)
- **Key elements:**
  - [ ] Booths (vinyl-covered box seats, neutral color)
  - [ ] Counter + stools
  - [ ] Counter mirror (flat plane — Sinclair uses this to watch the witness)
  - [ ] Overhead fluorescents (institutional)
  - [ ] Cook visible through kitchen pass-through (very low-poly, back turned)
  - [ ] Coffee mug (cylinder primitive)

---

### E15 — Lieutenant Grant's Office [P1]
- **Use:** S02E05 (Ch.5), recurring in projected seasons
- **Key elements:**
  - [ ] Office box geometry
  - [ ] Desk + 2 chairs (box primitives, desk larger — authority)
  - [ ] Horizontal-stripe window blind (flat plane with stripe texture, closed, light bleeding through)
  - [ ] Coffee cup (cylinder — always present)
  - [ ] Document folders on desk (flat plane stacks)
  - [ ] Commendation frames on wall (flat planes, small)

---

### E16 — Waterfront Loading Docks [P1] (Ch.6 / S02E06)
- **Key elements:**
  - [ ] Shipping container stack (box primitives x8–10, staggered heights and positions)
  - [ ] Sodium lamp pole (cylinder + cone shadow, orange point light)
  - [ ] Ground plane (industrial, wet asphalt + dock concrete)
  - [ ] Loading bay walls (flat geometry with bay door openings)
  - [ ] Wooden pier (flat plane, plank texture, extending into water)
  - [ ] Cinder blocks at pier end (small grey box primitives x3)
  - [ ] Dark water plane (reflective, very low wave animation)
  - [ ] Fog layer — DENSE (same as E01 fog but higher opacity)
  - [ ] White van (see V01)

---

### E17 — The Bridge (Projected — Ch.7–8 flashback) [P2]
- **Key elements:**
  - [ ] Bridge roadway plane (wet, rain-slicked)
  - [ ] Steel railing geometry (box profile)
  - [ ] Rain particles
  - [ ] Sodium street lamp (single)
  - [ ] Night city skyline at distance (flat cutout / skybox)

---

## CHARACTERS

### C01 — Detective Adrian Kane [P1]
- [ ] Base mesh (~1000 tris, low-poly)
- [ ] Texture atlas 512×512 (coat, suit, face)
- [ ] Bandage arm variant texture (Ch.5 onward)
- [ ] Bite wound with cold-blue tint variant (Ch.5–6 progression)
- [ ] Breath particle emitter (outdoor scenes)
- [ ] Animation set: idle, walk, run, crouch, sleeve-roll, weapon-check, punch, tackle

### C02 — Evelyn Sinclair [P1]
- [ ] Base mesh (~1000 tris)
- [ ] Texture atlas 512×512 — burgundy coat version (Ch.1–4)
- [ ] Texture atlas variant — dark navy coat version (Ch.5+)
- [ ] Bruise cheekbone variant texture (Ch.5 opening)
- [ ] Animation set: idle, walk, composed-stance, shoulder-tense (bass-sensitivity tell), check-exits ritual

### C03 — Tony DeMarco [P1]
- [ ] Base mesh (~800 tris)
- [ ] Club manager look (suit, slightly disheveled)
- [ ] Decapitated variant (headless seated pose — required for Ch.1 apartment scene)
- [ ] Head prop (separate mesh — the rolling head)
- **Note:** DeMarco appears only in S01E02; the head prop is reused as crime scene evidence.

### C04 — Max (face unseen until direct contact) [P1 mesh / P2 direct appearance]
- [ ] Dark coat mesh — **silhouette identical to Kane** (important design choice)
- [ ] Texture atlas 512×512 (grey-green coat, precise hair)
- [ ] Jaw/temple vein overlay (P2 — Ch.9–10 escalation variant)
- [ ] Cold skin variant (P2 — Ch.11 partial claiming variant)
- [ ] Animation: audience-addressing idle, deliberate-name usage (slow head turn), listening pause

### C05 — Voss [P1]
- [ ] Base mesh (~900 tris)
- [ ] Violet-black suit texture
- [ ] Ring animation (wrist-rotate when frustrated)
- [ ] Animation: theatrical idle, sudden-stillness (Lich override freeze)

### C06 — Lt. Marisol Grant [P1]
- [ ] Base mesh (~700 tris)
- [ ] Professional suit texture
- [ ] Coffee cup always in hand or on desk (linked prop)
- [ ] Animation: seated authority, leaned-forward listening

### C07 — Dr. Harlan Cho [P1]
- [ ] Base mesh (~700 tris)
- [ ] White lab coat variant (work) + shirtsleeve variant (Ch.6 night scene)
- [ ] Glasses prop (small wire-frame geometry)
- [ ] Animation: methodical lab work, glasses-removal (thinking tell)

### C08 — Officer Rook Alvarez [P2]
- [ ] Base mesh (~700 tris)
- [ ] Patrol uniform texture
- [ ] Animation: upright-posture, compliance-flicker (brief near-vacant expression)

### C09 — The Wrong-Cold Homeless Man [P1]
- [ ] Very simple mesh (~400 tris)
- [ ] Layered clothing texture (worn, layered)
- [ ] Branching vein texture overlay at throat (dark, ink-under-paper)
- [ ] Wrong-cold skin tint (slightly blue-grey in diffuse)

### C10 — Stitched-Mouth Attacker [P1]
- [ ] Base human mesh (~600 tris) with bind-pose offsets at hip/shoulder (~5–10 degrees)
- [ ] Stitch-mouth texture overlay (dark zigzag on face)
- [ ] Low-framerate keyframe animation (puppet effect — every 3rd frame, no smoothing)

### C11 — Generic Patrons / Club Crowd [P1]
- [ ] Billboard sprite sheet (12 variants, animated at 12fps)
- [ ] Use as background population for club scenes, street scenes

### C12 — Generic Officers / Uniforms [P1]
- [ ] Very low-poly base (~400 tris)
- [ ] Patrol blue texture
- [ ] Two or three variants

### C13 — Mirror Shadow Figure (Lich Indirect Presence) [P1]
- [ ] Very low-poly silhouette mesh (~200 tris)
- [ ] Single dark material (near-black)
- [ ] Human-adjacent proportions with one deliberate wrong proportion (arm length / neck angle)
- [ ] Render only in mirror camera layer — NEVER in primary scene camera
- [ ] Animation: static (it does not move while being observed)

### C14 — The Lich Lord (Full Reveal) [P2]
- [ ] Mesh (~1000–1200 tris — same tier as main characters for the reveal's gravity)
- [ ] Archaic robes with markings pattern integrated into fabric texture
- [ ] Cold-void skin (pale, no warmth in diffuse)
- [ ] Breath-fog effect scaled up (generated by proximity, not environment)

### C15 — Dock Runner [P1]
- [ ] Very low-poly (~400 tris)
- [ ] Gloves noted (design detail from prose)
- [ ] Compliance-walk animation (purposeful, vacant — no hesitation motion)

---

## PROPS

### P01 — The Markings / Sigil Texture [P1]
- [ ] 512×512 tileable UV texture (diffuse)
- [ ] 512×512 normal map variant
- [ ] Versions: light-etched, dark-painted, gold-inlaid
- **CRITICAL CONSISTENCY:** Same texture across all environments. Scale varies per context.

### P02 — The Vial [P1]
- [ ] ~60 tris mesh (cylinder, tapered, metal cap disc)
- [ ] Dark fluid material (low albedo, semi-transparent, absorbing rather than reflective)
- [ ] Particle emitter: sinking cold-blue breath-puff (2–3 particles, very low count)
- [ ] Condensation texture animation (UV-scrolling water-bead overlay)
- [ ] Fridge row configuration (instanced mesh, arranged in grid on fridge shelf interior)

### P03 — The Black-Framed Mirror [P1]
- [ ] Frame mesh (box profile, ~100 tris, markings normal map)
- [ ] Mirror plane (flat, reflection shader, -10–15% desaturation in reflection camera, 2–3 frame delay)
- [ ] Mirror camera (second render camera — sees the room from mirror's POV)
- [ ] C13 (shadow figure) placed in mirror-camera scene only
- **This is the most technically complex prop in the production.**

### P04 — The COME BACK Note [P1]
- [ ] Flat plane, paper texture
- [ ] Text: "COME BACK" (deliberate handwriting texture, capital letters)
- [ ] Stained variant (blood-stained edge for the Ch.1 version between Tony's teeth)

### P05 — The Polaroid (YOU STILL GRAB SLEEVES) [P1]
- [ ] Flat plane, Polaroid photo proportions
- [ ] Photo texture: desk scene (Kane's angle)
- [ ] Border text: "You still grab sleeves." (handwriting texture — same hand as P04)
- [ ] White border must look "too clean" against the aged case box

### P06 — The Case Box [P1]
- [ ] Cardboard box geometry (~30 tris)
- [ ] Aged cardboard texture with reinforcing tape detail
- [ ] Faded label decal (Kane's handwriting — no readable text needed)
- [ ] Interior files visible when open (stacked flat planes)

### P07 — Cho's Family Charm [P1]
- [ ] Tiny gold charm (~20 tris) on thin chain geometry
- [ ] Gold emissive material
- [ ] Fall animation (from microscope stand to tile floor)
- [ ] "Nudge before fall" animation (very slight movement before the fall — ambiguous supernatural/gravity)

### P08 — Lab Equipment Set [P1]
- [ ] Microscope (~80 tris iconographic)
- [ ] Centrifuge (~60 tris)
- [ ] Reagent strips (flat plane, small)
- [ ] Test tubes / sample tubes (cylinder primitives)
- [ ] Steel tray (flat box + lip geometry)

### P09 — The White Van [P1]
- [ ] Box body + cylinder wheel primitives (~80 tris total)
- [ ] Plain white texture, no logo
- [ ] No window detail (opaque or near-opaque glass material)

### P10 — Kane's Badge [P1]
- [ ] Flat hex/shield plane (~10 tris)
- [ ] Gold emissive material with shield shape
- [ ] Used in hand (Kane holding it) and belt-clip position

### P11 — Kane's Pistol [P1]
- [ ] ~50 tris semi-automatic geometry
- [ ] Matte black material
- [ ] Animation states: holstered, drawn, checked, aimed, fired

### P12 — Evidence Markers [P1]
- [ ] Yellow triangular prisms (~10 tris each)
- [ ] Yellow emissive material
- [ ] Number decal (1–8 variants)
- [ ] 6–8 instances used in apartment crime scene

### P13 — The Cooler Case [P1]
- [ ] Hard plastic box geometry with latch detail (UV-textured)
- [ ] Carried by dock runner in Ch.6

### P14 — Tony DeMarco's Head (Prop Version) [P1]
- [ ] Low-poly head mesh matching C03 topology
- [ ] Roll physics / animation (bounces from desk, lands face-up)
- [ ] Used only in Kane's apartment discovery scene

---

## VFX SYSTEMS

### VFX01 — Breath Particle System [P1]
- Cold-blue-white, 3–5 particles per breath cycle, upward drift for human breath, downward drift for vial cold
- Used by: all characters in exterior December scenes

### VFX02 — Bass Screen Pulse [P1]
- Post-process: screen-edge darkening (vignette breathe), 2–4 frames per pulse, magnitude barely perceptible on first view
- Synced to diegetic bass note in club scenes
- Slightly more pronounced when a character experiences obedience reflex

### VFX03 — Vial Centrifuge Rejoin [P1]
- Material UV animation on test tube: gradient (separated bands) slowly dissolves to solid (uniform fluid)
- 3–5 second duration, no particles
- Used once in S02E04

### VFX04 — Cold-Blue Skin Tint [P1]
- Material parameter animation on Kane's forearm (bite area) and contaminated persons
- Blends from normal skin tone to slight blue-grey over time
- Used on: Kane Ch.5+, wrong-cold homeless man Ch.2, dock runner Ch.6, projected Max Ch.9+

### VFX05 — Mirror Reflection Layer [P1]
- Second render camera at mirror position
- Desaturated -10–15% relative to primary camera
- 2–3 frame delay on reflection feed
- C13 (shadow figure) visible in mirror camera only

### VFX06 — Whispering Audio + Charm Fall (Cho Prologue) [P1]
- Not a VFX system — sound design. But the charm's very slight pre-fall movement is a material animation:
  - Tiny oscillation on the chain's endpoint (± 1mm) before the fall
  - Stop at fall moment — abrupt, not physically caused

### VFX07 — Low-Framerate Puppet Animation [P1]
- Applied to C10 (stitched-mouth attacker) and contaminated users
- Every 3rd keyframe, no smoothing between — creates stop-motion effect
- Very cheap to implement in Unreal (just increase the animation update interval)

---

## AUDIO CUES

### A01 — The Bass Command Tone [P1]
- Low-frequency subsonic pulse, approximately every 4 seconds
- Below normal music mix; felt rather than heard
- Present in all scenes with Lich influence; barely perceptible in Ch.1–4; audible to Sinclair (and audience) from Ch.4 onward
- Synced to VFX02 (bass screen pulse)

### A02 — December City Ambient [P1]
- Light rain or dry wind, depending on scene
- Distant traffic hiss, sodium hum
- 2–3 loop variants for variety

### A03 — Club Music (Velvet Abyss Diegetic) [P1]
- Heavy slow electronic/industrial, 80–90 BPM
- Bass-dominant
- Cut sharply when Voss seizes the comms channel in S01E05

### A04 — Jazz (Jazz Bar Diegetic) [P1]
- Sparse, modal, dark
- Low volume — background presence, not featured music
- Stops when the ambient shifts in the alley scene

### A05 — Morgue Ambient [P1]
- HVAC hum, refrigeration cycle sounds, very distant traffic
- The "whispering" (Ch.6): processed white noise with subtle formant filtering — voice-shaped but not intelligible
- Silence when the charm falls (abrupt ambient cut)

### A06 — The Silence [P1]
- The body-cam footage silence (before the thing climbs out): ambient sound fades to near-zero over 3 seconds, then holds
- The mirror room silence: no score during the mirror beat
- Kane's apartment discovery: no score, only breath and floorboard

### A07 — Hardboiled Score (Non-Diegetic) [P1]
- Noir jazz texture for investigation/character scenes: sparse, modal, guitar + muted trumpet + brushed snare
- Electronic drone for horror escalation scenes (replaces or underlays the jazz)
- Percussion-forward for action sequences (irregular rhythm, no heroic swell)

---

## REUSE MATRIX (Quick Reference)

| Asset | S01 | S02 | S03+ |
|---|---|---|---|
| E01 City Street base kit | Every outdoor scene | Every outdoor scene | Every outdoor scene |
| E02 Velvet Abyss Exterior | E01–E02, E04, E05, E06 | — | Projected return |
| E03–E06 Club Interiors | E06 partial | E01, E02 primary | Projected return |
| E13 Morgue | — | E04, E06 | Recurring |
| C01 Kane | All | All | All |
| C02 Sinclair | E03–E06 | All | All |
| P01 Markings texture | E06, E06 | E01, E02 | Projected |
| P02 Vial | E06 (pocket) | E01–E06 | Recurring |
| P03 Black Mirror | — | E02 | Projected return |
| A01 Bass Tone | E04+ | All | All |
