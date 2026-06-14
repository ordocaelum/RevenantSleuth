# REVENANT SLEUTH — Props and Motifs Reference
**Production Reference for Unreal Engine / Blender**
*VFX-light, low-poly-friendly. Every recurring prop and motif is described with both narrative purpose and a lean implementation strategy.*

---

## 1. THE VIAL — "Essence"

### Narrative Role
The MacGuffin. The drug. The payload. The key. The vial is the story's most loaded object — it appears in nearly every chapter and escalates in significance with each appearance.

### Physical Description (Per Prose)
- **Container:** A small glass vial, approximately 50ml, with a metal seal and a crack-able stopper.
- **Fluid color:** "Not quite black and not quite red — old blood diluted with oil." Under direct light, the fluid does not reflect cleanly; it *discourages* light, as if absorbing rather than bouncing.
- **Temperature:** The vial is always cold. Not cold like something from a refrigerator — cold like something that doesn't want to participate in thermodynamics. When placed on a metal tray, **condensation forms instantly**. The steel darkens where the chill spreads.
- **Behavior:** The fluid inside resists separation (the centrifuge bands rejoin). It responds to being observed with something that feels like awareness. When opened, the air above it grows **thin and faintly floral** — sweet, dusty, funeral.

### Low-Poly Model
- **Geometry:** A simple cylinder primitive with slightly tapered ends. Metal cap (a flat disc + very short cylinder collar). Total: ~50–80 tris.
- **Material — the fluid:** A dark red-brown semi-transparent material with an emissive tint that reads as slightly **absorbing** (lower albedo than surrounding environment). This is the one shader where the fluid should look *wrong* — slightly less reflective than glass physics would suggest.
- **The cold effect:** A particle emitter at the base of the vial — very low count (2–3 particles), small, slow, cold-blue-white. Like breath-fog but downward, sinking rather than rising. This is the key visual tell.
- **Condensation:** Animated texture overlay on the glass — gradual water-bead accumulation on the cylindrical surface. Can be a scrolling normal map or a UV-animated decal.

### Recurring Scene Use
| Chapter | Context | Visual Emphasis |
|---|---|---|
| Ch.4 | Industrial fridge — rows of vials | Volume: the horror is quantity. One box of vials; rows of cold points all bleeding chill through the seals. |
| Ch.5 (motel) | In Kane's coat pocket | Felt rather than seen — close on Kane's hand instinctively moving away from the pocket |
| Ch.5 (morgue) | On steel tray, being tested | The centrifuge-rejoin sequence is the key VFX beat |
| Ch.5 (morgue) | Locked in Cho's fridge | Same cold-blue emissive at the fridge seal as the basement fridge |
| Ch.6 (projected Ch.7+) | Dock runner's cooler | New acquisition vector |

### The Centrifuge-Rejoin VFX Beat (Ch.5 — HIGH PRIORITY)
This is the story's first explicit K3 confirmation. Execution:
1. Cho spins the sample — centrifuge hum, 30 seconds.
2. He opens it: bands visible in the test tube (subtle gradient, dark-to-light).
3. Camera holds on the tube.
4. The bands slowly blur — a very slow dissolve on the gradient texture, over 3–5 seconds.
5. The fluid is uniform again, as if it was never separated.
6. Cho's reaction: jaw clenches. He sets the tube down carefully.

VFX approach: this is a **material animation only** — no particles, no complex simulation. The gradient UV-animates back to solid. Extremely cheap.

---

## 2. THE MARKINGS / SIGILS

### Narrative Role
The command architecture of the Lich's system. These are not decoration — they are infrastructure. Wherever they appear, the obedience mechanism has been installed.

### Physical Description
- Curved, repeating lines that suggest a language but are not a recognizable one.
- "Archaic" — they read as older than any modern written language.
- At first glance, they look like unusual art deco pattern — integrated into pillar engravings, door frames, gold trim.
- Up close, the repetition is too precise for hand-carving. They were made with purpose.

### Visual Consistency (Production Rule)
The markings are **one UV-mapped texture** used across all locations. Same pattern, different scales and materials:
- Velvet Abyss pillars: large scale, etched shallow, paint-dark
- Corridor double doors: medium scale, engraved deep into metal, gold-highlighted
- Basement walls: smaller, painted in a darker medium, almost not visible until lit correctly
- Mirror frame: smallest, densest, covering the whole frame surface
- Future projected appearances: the dock cargo containers (projected Ch.6/7), Max's personal space (projected Ch.7+)

**Production asset:** one 512×512 tileable normal map / diffuse texture. Scale to context.

### Depiction Tone Rule
- **Ch.3 (Evelyn noticing):** Shown as slightly odd-looking design elements. Not alarming yet.
- **Ch.4 (red velvet corridor + basement):** The camera lingers on them — slightly longer than natural — establishing the feeling that something is watching through them.
- **Mirror frame:** The most concentrated appearance. The density of the markings here should read as *intentional saturation* — they cover every surface of the frame.
- **Never explain the markings on-screen before K2 is confirmed.** Characters may point at them; they cannot decode them.

### Low-Poly Depiction
Since geometry carving is expensive at low-poly, all marking appearances are **texture/normal map only**. The shape is the texture; the geometry remains flat. This is correct.

---

## 3. THE BLACK-FRAMED MIRROR (Basement, Ch.4)

### Narrative Role
The Lich's watching eye. The mirror is the story's most supernaturally charged prop — the one place where the Lich's presence is almost visible. It shows something that isn't in the room.

### Physical Description
- **Frame:** Black lacquered wood or black-painted cast iron. Heavy, ornate in its geometry — complex profile for a low-poly environment. The entire frame surface is covered in the markings (densely carved or inlaid).
- **Glass:** Dark-tinted. Not opaque but not fully transparent either — like a one-way mirror that isn't fully committed to the principle.
- **Size:** Wall-mounted. Large — roughly human-sized (5–6 feet tall, 3 feet wide). A mirror you could step through if the physics cooperated.

### The "Wrong Shape" in the Reflection (Ch.4 — KEY VISUAL BEAT)
When Evelyn directs Kane's attention to the mirror, they see a shape in the reflection that is not present in the room:
- The shape is **low-poly, dark, hunched** — human-adjacent but wrong in at least one proportion (arms too long, neck at an angle, posture that suggests forward lean but toward the viewer, not away).
- It does not move while they watch. It is simply *there*, in the part of the reflection that corresponds to where the viewer would stand.
- When the scene cuts away and returns, it is gone.

**Production approach:**
- The mirror is rendered as a **second camera** with a slightly different color temperature (cooler, desaturated by 10–15%) and a 2–3 frame delay on its reflection feed.
- The "wrong shape" is a separate low-poly model, rendered only in the mirror camera's layer, placed behind the viewer's POV in the mirror's world-space.
- No model is visible in the primary scene — only in the mirror.
- The color temperature difference makes the reflection feel slightly wrong even before the shape is visible.

---

## 4. THE NOTES (Max's Messages)

### Narrative Role
Max's signature. He doesn't just kill — he leaves proof that he was there, that he knows where Kane lives (literally and psychologically), and that Kane is expected.

### Physical Descriptions
**Note #1 — "COME BACK" (Ch.1)**
- Paper: single sheet, slightly stained. The stain is from the context (between Tony's teeth).
- Ink: black, clean, precise. Not handwritten in the emotional sense — not scrawled. Printed-looking by hand, with deliberate letter-spacing.
- Text: COME BACK. Nothing else.
- The note is a summons. The capital letters are not shouting — they are formal.

**Note #2 — "YOU STILL GRAB SLEEVES" (Ch.6)**
- A Polaroid photograph showing Kane's own desk, from Kane's own angle.
- On the white border: "You still grab sleeves." Written in black ink, same deliberate hand.
- The horror: this is not a threat. It is an intimacy. Max knows Kane's angle, his height, his sight-line.

### Visual Consistency
Both notes share:
- The same **handwriting texture**: consistent letter shapes, deliberate spacing. Not calligraphy; not scrawl. Controlled.
- The **COME BACK** note can appear large in frame — Kane reading it, the letters filling the frame. Good for a thumbnail/key art moment.
- The Polaroid note should be shown in contrast to the case box contents — the "too-clean" white border against aged cardboard.

---

## 5. STITCHING / REASSEMBLED BODIES

### Narrative Role
The Lich's most literal signature. Bodies that have been taken apart and put back together — not to restore them, but to *configure* them. The stitching is not medical. It is *architectural*.

### Visual Descriptions
**Family in the car (Ch.1 — body-cam footage):**
- Not ritualistic exactly. More like someone had tried to put them back together in the dark, impatient and angry.
- **Production note:** This is seen only on a monitor screen (in-game computer screen render) — which naturally limits the level of horror. This is correct — the body-cam filter does the work. Desaturated, slightly washed, the grain of night-vision footage. Detail is deliberately limited.
- Low-poly is fine here: shapes of bodies, no fine detail. The horror is in the *arrangement*, not the anatomy.

**Stitched-mouth attacker (Ch.4):**
- A human figure with the mouth sutured closed — thick black thread, visible and deliberate. The stitches are not subtle.
- The body moves with "wrong angles" — joints at slightly off positions, as if the assembly was done from a description rather than observation.
- **Production approach:** The character model shares the base human mesh but with:
  - A dark stitched-mouth texture overlay on the face
  - A slight rotation offset at the hip joint and shoulder joint (maybe 5–10 degrees from normal) — enough to read as wrong, not enough to break the model
  - Movement animation: stiff, jerky (low-framerate keyframe animation — every 3rd frame, not smoothed) — the marionette effect

### Low-Poly Implementation
- **The stitching** on the mouth attacker: a texture overlay, not geometry. A dark zigzag pattern on the face diffuse.
- **The wrong-angle posture:** achieved through animation rigging — the bind pose is slightly "off" from human neutral.
- **The movement:** low-framerate keyframe animation (puppet-stop-motion effect) is extremely cheap and more effective than smooth animation for conveying inhumanity.

---

## 6. BODY-CAM FOOTAGE EFFECT

### Narrative Role
The medium through which we experience the Ch.1 horror without showing it directly. The footage is the story's opening horror frame — it establishes that this is a city where the dead do things.

### Visual Treatment
- **Footage overlay:** A subtle VHS/body-cam frame — slight scan lines, corner vignette, timestamp display in the upper corner (no actual numbers needed — just the visual noise of a clock).
- **Color:** Desaturated, night-exposure white balance. Everything looks slightly washed-out.
- **Camera movement:** The footage should be *shaky in the wrong moments* and *unnaturally still in the right ones* — the rookie tries to hold steady, then fails.
- **Monitor render:** The footage is seen on a screen in the bullpen, which means it is seen as a **texture on a flat screen primitive** — the VHS/scan-line treatment is applied to the texture, not the scene. Very cheap.

---

## 7. THE RECURRING SIGNATURES — VFX SUMMARY

### Quick Reference Table

| Signature | VFX Approach | Cost | Where Used |
|---|---|---|---|
| **Heat theft / cold** | Particle emitter (sinking cold-blue breath-puff), ambient color temp shift to blue on nearby surfaces | Very low | All vial scenes, bite wound, basement fridge |
| **Obedience to bass** | Post-process screen-pulse (very subtle, 1–2 frame) synced to diegetic bass note; character posture snap | Low | Ch.4 bouncers, Ch.5 kneeling user, Ch.6 dock runner |
| **Stitching / reassembly** | Texture overlay (zigzag stitch lines), joint-offset in bind pose, low-framerate animation | Low | Ch.1 footage, Ch.4 attacker |
| **Mirror watching** | Second render camera (mirror layer), cooler color temp, shape silhouette in mirror layer only | Medium (two cameras) | Ch.4 mirror room |
| **Archaic court diction** | No VFX — this is dialogue/audio only; character animation note: slower delivery cadence | None | Max, Voss (light), Ch.11 Lich |
| **Aristocratic patience** | Camera behavior — long holds, no cuts; the environment waits | None (camera/edit) | All Lich-adjacent scenes |

### The Bass Pulse — Detail
The obedience reflex is tied to a specific bass frequency. In the video adaptation:
- The diegetic music in club scenes should have an audible low-frequency pulse that the viewer can *feel* (subwoofer frequency if possible in the audio mix).
- The visual correlate: at the peak of each bass hit, a very subtle **screen-edge darkening** pulse (like a gentle vignette that breathes with the music). Duration: 2–4 frames. Magnitude: nearly imperceptible on first viewing.
- When characters respond to the command signal, this pulse is slightly more pronounced — the screen darkens, the character moves, the screen returns to normal.
- **Reveal discipline:** In Ch.1–4, the pulse is present but the audience may not consciously notice it. In Ch.5–6, Sinclair's reaction (shoulder tense, involuntary pull) gives the audience the cue to go back and see it. In Ch.7+, the pulse becomes legible as intent.

---

## 8. THE BRIDGE (Props and Set, Projected Ch.7–8)

### Narrative Role (Projected)
The Bridge incident is the event that broke the Kane-Max partnership. The exact details are unknown through Ch.6, but Kane associates it with a specific physical memory: rain on steel, his hand wrapped around a sleeve, boots skidding, Max's voice calm as surgery: *"Let him go. He's already decided."*

### Visual Requirements (Projected)
- A **rain-slick suspension or pedestrian bridge** — city setting, December. Wet steel railings.
- One figure at the rail, facing outward.
- Kane's hand extended, gripping fabric.
- Max at Kane's side, close enough to whisper, calm as surgery.
- The moment of letting go (or not) — to be determined by the author.

### Low-Poly Notes
- The bridge is a simple environment: flat roadway plane, steel railing geometry (box-profile), cable pylons or arch (box/cylinder primitives).
- The emotional weight is entirely in the two characters and the lighting: rain particles (simple point emitters), sodium street lamp backlighting the scene.

---

## 9. MISC PROPS (Supporting)

| Prop | Description | Low-Poly Approach |
|---|---|---|
| **Kane's badge** | Standard detective shield. Gold tone. Shown held in hand or clipped to belt. | Flat hex/shield-shaped plane, gold emissive material |
| **Kane's pistol** | A standard service semi-automatic. He checks it often but rarely fires. | ~50 tris, semi-realistic proportions, matte black |
| **Cho's family charm** | A small metal charm on a chain — "keeps the bad air away." It falls in Ch.6. | ~20 tris gold plane, thin cylinder chain |
| **The white van** | Plain, no logo, cargo van type. Appears Thursdays and Mondays at the club, and at the dock. | Box + cylinder wheels, plain white texture |
| **Evidence markers** | Yellow numbered plastic triangles. Appear at the apartment crime scene. | 10-tri triangle prisms, high-visibility yellow emissive |
| **The cooler case (dock, Ch.6)** | Hard plastic carrying case, latched. Used to transport vials. | Box primitive, flat plastic material, handle detail as UV texture |
