# REVENANT SLEUTH — Locations Reference
**Production Reference for Unreal Engine / Blender**
*All assets assume LOW-POLY construction. Notes indicate where silhouette, lighting, and color do the heavy lifting instead of geometry.*

---

## 1. THE VELVET ABYSS (Club)

### Exterior
**Mood:** A wound in the city. Invitation and threat simultaneously. The building breathes — neon pulses like a heartbeat, not a sign.

**Color/Lighting:**
- Primary neon: **deep purple** and **blood red**, mounted above entrance and along the facade's upper lip.
- Street-level: wet asphalt reflecting the neon as smeared bruises. Fog optional but preferred.
- The entrance door glows from within with warm amber-gold — the only "inviting" note, which makes it worse.
- December cold: visible breath. Every character's breath should be rendered as a subtle particle.

**Set Dressing:**
- Brick facade, possibly pre-war, re-clad in black painted panels with the club name in no-frills neon lettering (not scripted, not cute — industrial).
- A line of patrons: silhouettes, not individuals. Low-poly crowd shader.
- Two bouncers (large, in black) flanking the entrance, cigarettes glowing.
- Security camera visible above the door — the club is always watching.

**Low-Poly Modeling Notes:**
- The facade can be a flat-plane brick texture with a few extruded panel shapes for depth.
- Neon is best achieved via emissive materials on simple tube-mesh shapes, not complex geometry.
- Wet asphalt: use a flat plane with a reflection shader and animated neon emissive overlay. No puddle geometry needed.
- Silhouette crowd: billboard sprites or very-low-poly mesh crowd, no individual detail.

**Camera/Blocking Notes:**
- Establish shot: wide, low angle from across the street. Club fills the upper-right third. Kane in foreground, small, watching.
- Approach shot: dolly-in from street level, neon blooming larger as we close.

---

### Interior — Main Floor
**Mood:** Controlled chaos. Hunger dressed up as freedom. Bodies moving because the bass told them to.

**Color/Lighting:**
- Purple wash from above (colored gel on generic ceiling rigs — low-poly lights).
- Pulsing strobes: low-frequency, synchronized with the diegetic bass. Every third beat, the room is lit; between beats, near-darkness.
- Smoke/haze: cheap particle system or billboarded plane layers. Never use volumetric fog for this — too expensive.
- Bar backlit bottles: the one warm light source, providing amber-gold contrast against the purple.

**Set Dressing:**
- Long bar, dark wood or black lacquer, running the left wall.
- Dance floor center: low-poly bodies as crowd, no individual faces needed.
- Booths along the right wall, red upholstery, gold piping.
- Speakers stacked at corners — visible, large, ostentatious. The bass has a physical presence; the speakers are its body.
- **The markings:** etched into pillar surfaces, door frames, and integrated into the decorative trim. They look like art deco gone wrong — until you look closely. Low-poly: use UV-mapped texture, not extruded geometry.

**Low-Poly Modeling Notes:**
- The dance crowd can be a billboarded sprite sheet animated at 12fps — sufficient for background mass.
- Booths: simple box geometry with red emissive-tinted material and gold edge highlight.
- Bar: flat countertop plane + simple stools.
- Speakers: black box primitives, stacked at angles.

---

### Interior — Red Velvet Corridor
**Mood:** The club's true face. This is not entertainment — this is architecture of control. Opulent, suffocating, wrong.

**Color/Lighting:**
- Deep red walls: actual velvet texture simulation or a dark matte red with specular highlight at eye level.
- Gold trim: emissive warm gold along door frames, wall panels, light sconces.
- Overhead light is sparse — single sconce every 8 feet, amber-warm. The spaces between are shadow.
- The floor is darker than the walls, which creates a sense of walking through a throat.

**Set Dressing:**
- Double doors at corridor end: heavy dark wood (or metal), gold engraving. The engravings are the markings again — but here they're explicit, formal, *deliberate*. Not "etched decor." These were made with intention.
- Wall panels between sconces: the markings repeat in subtle relief. Barely visible at first glance.
- No seating. This corridor has no purpose except passage.

**Low-Poly Modeling Notes:**
- The corridor can be a simple tunnel (box with UV-mapped texture) with a few low-poly sconce props.
- The double doors: flat plane with engraving as a normal map / emissive overlay. No need to model the engravings as geometry.
- The "throat" effect: achieved via lighting — warm amber pools every few feet, total darkness between. No geometry required.

---

### Interior — Basement "Factory"
**Mood:** Industrial horror. This is where the product is made, but "product" means something else here. The word "factory" is exact — it is a place of manufacture, and the raw material is human.

**Color/Lighting:**
- Harsh industrial fluorescent overhead (cool white, clinical). Flickering optional but effective — one or two tubes at 75% function.
- Metal tables catch and reflect the light — stainless steel, high-specular even in low-poly.
- The drains in the floor: visible. Dark. Significant.
- The fridge unit: a cold blue-white glow emanating from its seal. This is the only supernatural light in the space — everything else is mechanical.

**Set Dressing:**
- Metal examination tables: three or four, with restraint points.
- **Bound users:** human figures seated/lying at the tables, slack-postured, swaying slightly. Their eyes are open. Their mouths move. They are not here.
- **The industrial fridge:** a heavy commercial unit with keypad lock. Behind the seal, cold fog leaks from the gap between door and frame. When opened: rows of vials, dark-red, the fluid absorbing rather than reflecting the overhead light.
- Tools on a side table: purpose ambiguous but clinical. Don't label them.
- **Drains in the concrete floor:** dark, slightly recessed. Stained at their edges.

**Low-Poly Modeling Notes:**
- Metal tables: flat box geometry with high-specular material. Restraint points: small cylinder primitives on edges.
- Bound users: very low-poly figures, no face detail needed — the horror is the *behavior*, not the face.
- Fridge: box primitive with emissive-tinted seal (blue-cold). The leaking-fog effect: simple particle emitter at the door gap, very low count.
- Drains: flat circular decal on floor plane. No geometry needed.

---

### Interior — Red-Lamp Side Room
**Mood:** Intimate horror. This is where they held Evelyn. The red lamp makes everything look like blood. The black-framed mirror is the room's most dangerous object.

**Color/Lighting:**
- A single red practical lamp: deep red, tungsten temperature, mounted above an armchair or wall bracket.
- The room is small — four walls, low ceiling. The red light fills it entirely, casting no shadows except at the corners.
- The **black-framed mirror** is the brightest reflective surface — it returns the red light but slightly *wrong*. The reflection is slightly delayed, slightly colder in hue.

**Set Dressing:**
- An armchair (red upholstery, dark wood frame) — where Evelyn was held.
- The black-framed mirror: large, ornate frame, wall-mounted. The frame is carved with the markings. The mirror surface appears normal until a character is in close proximity — at which point a *shape* appears in the reflection that is not in the room.
- A small side table with no clear purpose. One item on it: a glass of water, untouched.

**Low-Poly Modeling Notes:**
- Mirror: flat plane with reflection shader. The "wrong shape" in the reflection is achieved via a separate render layer or a second hidden camera — not a complex mesh. The shape should be a dark low-poly silhouette: human-adjacent, hunched, watching.
- Frame: simple box profile around the mirror plane. Markings as normal map.
- Red light: single point light with a red color and short falloff radius. Very cheap to render.

---

## 2. KANE'S APARTMENT

### Exterior — Building
**Mood:** A tired man's home. The building apologizes for itself.

**Color/Lighting:**
- Brick facade: old, stained, slightly dark from years of city exhaust.
- A single lobby light visible through a ground-floor window: it flickers. Not haunted — just neglected.
- Streetlight outside: amber sodium lamp, creating a pool of warm yellow against the cold December dark.

**Low-Poly Modeling Notes:**
- Flat-face brick building: 3–5 story simple geometry. Extruded window sills (flat planes). No architectural detail except the weathered brick texture.
- The flickering light: animated emissive material at 80–100% intensity cycling.

---

### Interior — Apartment / Living Room
**Mood:** Functional minimalism. This is a man who doesn't invest in comfort because comfort makes you slow.

**Color/Lighting:**
- Ambient: night light through curtained windows — city glow, a mix of sodium amber and far-off neon.
- When Kane enters with a flashlight: a hard white beam cutting through dark, revealing furniture in harsh shadows.
- The desk lamp (if on): single directional warm pool.

**Set Dressing:**
- A desk: file folders, a lamp, a coffee mug. **The case box** on the shelf above — cardboard, reinforced tape, faded handwriting label.
- A chair (the scene-of-crime chair): where DeMarco's body was seated.
- Bookshelves or filing cabinet: functional, not decorative.
- The floor: a rug (now stained) over bare wood. Evidence markers (yellow plastic triangles) after the crime scene.

**Low-Poly Modeling Notes:**
- The apartment can be built from 8–10 primitive shapes: floor, ceiling, four walls, desk, chair, bookcase, rug.
- The case box: a simple box primitive with a paper-label decal on its face.
- Evidence markers: bright yellow triangular prisms — simple geometry, high visibility.

---

## 3. THE JAZZ BAR (Ch.2)

**Mood:** The city's hidden lung. No sign. No pretense. Just amber light and tired music and the understanding that some places exist to give people a reason not to disappear.

**Color/Lighting:**
- **Single amber bulb above the door** — exterior only. The whole exterior is dark except this one warm point.
- Interior: low amber throughout. Candles optional. No overhead fluorescents.
- Bar mirror behind the bottles: Kane studies Evelyn's reflection here first. The mirror is unadorned, honest — contrast with the Velvet Abyss mirror.
- Smoke haze in the air: same sprite-plane technique as the club, but slower, older.

**Set Dressing:**
- A bar: dark wood, worn smooth. Two stools visible in our shots (the rest of the bar can be implied).
- Jazz musician in the background: a single figure, low-poly, silhouette against a dim back wall. Instrument (trumpet or upright bass) identifiable by shape.
- No crowd — maybe two or three other patrons, shapes in shadow.
- Bottles backlit on bar shelves: the amber glow source.

**Low-Poly Modeling Notes:**
- Very sparse — the emotional weight is in the lighting and the two actors (Kane and Evelyn). The bar itself can be a flat counter plane + stools.
- Jazz musician: low-poly figure, no face detail, just shape + instrument silhouette.

---

## 4. THE MOTEL (Ch.5)

**Mood:** Guilty light. Every surface looks like it remembers something it shouldn't. This is not a sanctuary — it is a controlled environment for people who can't go home.

**Color/Lighting:**
- **Yellow** everywhere: yellow shade, yellow walls, yellowed curtains. The palette is literally sickly.
- Rain on the window: patient tapping. Exterior ambient light is sodium yellow from a parking lot lamp.
- One lamp on the nightstand: warm but not enough to fill the room. Significant shadow areas.

**Set Dressing:**
- Two double beds (standard motel layout).
- A scarred nightstand with the lamp.
- A bathroom door ajar: white tile, harsh white light inside (contrast with the yellow exterior).
- Curtains that don't fully close: a persistent gap through which the parking lot lamp bleeds.

**Low-Poly Modeling Notes:**
- The room is a box. Beds: flat rectangular planes with simple pillow geometry. Nightstand: small box primitive.
- The yellow atmosphere is achieved entirely through lighting and texture tint — no complex geometry.

---

## 5. THE MORGUE / AUTOPSY SUITE

**Mood:** Science trying to hold the line. The room smells of antiseptic bullying rot into silence. It's the most rational space in the story, and it's failing.

**Color/Lighting:**
- Primary: harsh overhead fluorescents (cool white, high intensity). This is the antithesis of the club — everything is visible, everything is clinical, nothing is hidden by shadow.
- The anomaly: when the vial is present, a subtle cold-blue tint bleeds into the nearest light source. Never dramatic — just *slightly* off. Wrong white balance.
- The fridge unit (Cho's personal lock-unit): same treatment as the basement fridge — cold-blue emissive at the seal.

**Set Dressing:**
- Autopsy table: stainless steel, center of the room. Drain below.
- Side counter: microscope, reagent strips, centrifuge (small lab unit). The vial sits on a steel tray here during analysis scenes.
- Cho's desk in the corner: legal pad, cold coffee mug, the family charm on its chain.
- The dedicated fridge (smaller unit, keypad-locked): against the back wall. Label reads nothing — Cho coded it.

**Low-Poly Modeling Notes:**
- The steel table: flat box, high specular metallic material.
- Lab equipment: simple cylinder + box combos (microscope, centrifuge). Iconographic rather than detailed.
- Cho's desk: flat plane + box geometry. The legal pad: a white rectangle. The charm: a tiny emissive gold point.

---

## 6. THE DINER (Ch.5)

**Mood:** A place that survived by never being special. Witness scenes need neutral ground — somewhere that doesn't threaten either party.

**Color/Lighting:**
- Overhead fluorescents (functional, institutional). Not mood lighting — operating room lighting.
- Coffee on the table: practical warm point.
- Bar mirror behind the counter: the mirror where Sinclair watches the witness from the rear booth.

**Set Dressing:**
- Plastic-covered menus on the tables. Coffee mugs (thick ceramic, functional).
- Booths: vinyl upholstery, neutral color (green or red, typical diner).
- A counter with stools.
- A cook visible through the kitchen pass-through: low-poly figure, back turned.

---

## 7. LIEUTENANT GRANT'S OFFICE (Precinct)

**Mood:** Institutional. The office is designed to project authority without warmth.

**Color/Lighting:**
- Fluorescent overhead with one window (blinds always closed — but light bleeds through the slats in horizontal stripes across the desk).
- A coffee cup that never empties: practical detail.
- Papers on the desk: folders, photos, the weight of bureaucracy made physical.

**Set Dressing:**
- A desk and two chairs (the power dynamic is built into the furniture placement).
- Blinds on the window — never opened.
- A small lamp on the desk.
- Diplomas / commendations on the wall: flat planes with small square decals.

---

## 8. WATERFRONT / LOADING DOCKS (Ch.6)

**Mood:** The city at its most industrial. This is where the machine shows itself without ornamentation.

**Color/Lighting:**
- Sodium lamp overhead: sickly orange-yellow. Everything is slightly jaundiced.
- Fog: dense ground-level fog. Use a plane-based fog layer, not volumetric (cheaper).
- The ocean: dark, flat, barely visible at the pier's edge. Reflections of dock lights.
- Headlights of the white van: cutting through fog, muted.

**Set Dressing:**
- Stacked shipping containers: 8–10 container primitives in staggered rows. Simple box geometry, different heights.
- A sodium lamp on a pole: single warm emissive point, cone shadow.
- The wooden pier extending into water: plank texture on a flat plane with slight warp for wear.
- Cinder blocks at the pier end: small grey box primitives.
- The white van: parked near loading bays. Very simple geometry — box + cylinder wheel primitives.

**Low-Poly Modeling Notes:**
- The whole dock scene can be built from boxes — containers, van, loading bay walls, lamp pole.
- The fog plane: a slightly transparent white/grey plane at knee-height, animated slow drift.
- The ocean is implied rather than modeled — a dark plane with minimal wave texture animation.

---

## CROSS-LOCATION NOTES

### The Color Temperature Gradient (Emotional Mapping)
| Location | Color Temperature | Emotional Register |
|---|---|---|
| The Velvet Abyss — exterior | Purple + red neon | Predatory invitation |
| The Velvet Abyss — interior | Purple + amber | Controlled seduction |
| Red velvet corridor | Warm amber (sparse) | Aristocratic menace |
| Basement factory | Cool white (clinical) | Industrial horror |
| Kane's apartment | Amber + city bleed | Exhaustion, violation |
| Jazz bar | Deep amber | Neutral ground, confession |
| Motel | Yellow (sickly) | Temporary sanctuary, guilt |
| Morgue | Cool white | Rational dread |
| Grant's office | Institutional white | Authority, political pressure |
| Waterfront | Sodium orange + fog | Cold truth, industrial scale |

### Reused Assets (Note Once, Use Many)
- **Vial prop** — used in basement, Kane's pocket, morgue. One model, multiple contexts.
- **Crowd silhouette sprites** — used in club exterior line, interior dance floor, diner background.
- **Kane's detective coat** — same model through all seasons; shows wear accumulation via texture variation.
- **The markings (sigil texture)** — the same UV-mapped texture used on pillars (club), corridor doors, basement walls, and the mirror frame. Consistency is the horror.
