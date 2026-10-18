# Art Production Reference

> Internal reference for generating Fifth Root artwork. Not player-facing game rules —
> see [16-accessories.md](16-accessories.md) for what these items actually do.

All 24 accessory and healing-item assets have already been generated from the prompts below
and are live in doc 16. Keep this page for regenerating a single item, or for adding new ones
in a style that matches what already exists.

---


You'll generate these externally. The single most important thing for a card game is that all 16 accessories look like they came from **one set** — so use the shared style block below on every prompt, changing only the item description.

## Shared Style Block

Paste this before each item prompt, unchanged, every time:

```
Single fantasy RPG inventory item icon, centered, three-quarter view.
Painterly hand-illustrated game-asset style with rich detail, warm hammered
gold trim, carved wood and living bark, woven vine, and inset glowing gem.
Palette limited to bark brown, deep forest green, and antique gold, with one
accent colour. Faint green Aether energy traces along the seams and joins.
Item only — no character, no hands, no ground, no cast shadow, no text,
no watermark, no border, no frame, no background tile.
Plain flat pure white background, item fully isolated.
```

Then append the item line. Set the accent colour per guild: **Ground** = moss green · **Fire** = ember orange · **Water** = pale blue · **Energy** = electric yellow · **Universal** = Aether green.

### Why the negatives matter

The first Copilot batch came back as a **contact sheet** — a 3×3 grid of items on individual textured background tiles with decorative frames and category banners. Those are unusable as game assets: the background bakes into the file and has to be cut out by hand.

The lines `no background tile`, `no border`, `no frame`, and `item fully isolated` are what prevent that. Generate **one item per image**, and never ask for a set or a sheet in the same prompt — asking for multiple items is what triggers the grid layout.

### Staying inside the world

The ROOT Kingdom has no forged steel, no plate helmets, no pointed wizard hats, no animal pelts, and no purple or pink gems. Everything is **grown**: wood, bark, vine, leaf, gold that looks poured rather than hammered, and Aether crystal in the four guild colours. If a generated item looks like it came from a generic fantasy dungeon, it does not belong here — regenerate it.

## Per-Item Prompts

**Root Band** — *accent: moss green*
> A woven bark forearm cuff, three strands of living root braided together, small green leaf buds sprouting where the strands cross, a single flat river stone set at the centre.

**Ember Ring** — *accent: ember orange*
> A thick copper finger ring shaped like a curled flame, the metal darkened as if forged and quenched many times, a small orange ember suspended and glowing inside the curl.

**Tideband** — *accent: pale blue*
> A smooth circlet of driftwood and polished blue river stone, worn at the temple, water endlessly beading and running along its underside without ever falling.

**Volt Brace** — *accent: electric yellow*
> A split ankle brace of dark wood banded with tarnished silver, the two halves not quite touching, a small arc of yellow lightning leaping continuously across the gap.

**Seedagon Charm** — *accent: Aether green*
> A small carved wooden pendant shaped like a sleeping seed sprite curled around a single sprouting seed, worn smooth from handling, a soft green glow from within the seed.

**Greenhouse Gloves** — *accent: moss green*
> A pair of worn canvas gardening gloves, soil-stained at the fingertips, bark patches sewn across the knuckles, tiny green shoots growing out of the seams.

**Patrol Lantern** — *accent: Aether green*
> A small hand lantern of bark and warped glass hung from a vine cord, containing not a flame but a slowly rotating mote of green Aether light.

**Rootweave Armor** — *accent: moss green*
> A heavy chest piece of interwoven living roots and thick bark plating, moss growing in the crevices, dense and immovable, with gold banding at the shoulders.

**Flameshod Boots** — *accent: ember orange*
> A pair of tall armoured boots in blackened gold, the soles cracked and glowing orange like cooling forge metal, faint heat shimmer rising from the heels.

**Tide Sigil** — *accent: pale blue*
> A flat circular medallion of pale blue crystal held in a driftwood frame, a spiral wave carved into its face, water running upward along the spiral against gravity.

**Storm Crown** — *accent: electric yellow*
> A narrow open circlet of dark twisted branches with upward-pointing tips, yellow lightning arcing continuously between the points above the wearer's brow.

**Aether Stone Pendant** — *accent: Aether green*
> A raw uncut green Aether crystal wrapped in fine gold wire, hanging from a braided vine cord, glowing from deep inside as though lit by something far away.

**Mageweave Cloak** — *accent: Aether green*
> A heavy hooded cloak of deep forest green, gold leaf-shaped clasps at the throat, hem tattered into leaf shapes, faint green Aether motes drifting off the edges.

**Fourfold Band** — *accent: all four*
> A single wide ring divided into four seamless quarters — bark brown, ember orange, pale blue, and electric yellow — each quarter a different material, joined by a thin gold seam.

**Counter Wrap** — *accent: Aether green*
> Layered vine and leather hand wraps, bound tight across the knuckles, a small green Aether stone knotted into the binding at the back of the wrist.

**Fifth Root Token** — *accent: gold, holographic*
> A heavy gold medallion shaped like a five-pointed root system radiating from a central seed, four roots polished bright and the fifth left dark and unfinished, deep green Aether pooling in the carved channels. Legendary treasure, warm inner light.

## Healing Item Prompts

Use the same style block, but add: `small consumable item, simple and readable at thumbnail size`.

| Item | Prompt line |
|------|-------------|
| Dewleaf | A single broad green leaf cupped to hold a large bead of dew that glows faintly |
| Rootbark Poultice | A folded bundle of bark and moss tied with vine cord, damp and freshly packed |
| Tidewater Vial | A small round glass vial of luminous blue water, stoppered with carved driftwood |
| Ember Root | A gnarled root with its broken end glowing orange like a lit coal |
| Sparksap | A vial of thick golden sap with tiny yellow sparks suspended and drifting inside |
| Seedagon Nectar | A tiny acorn-shaped flask of warm amber nectar with a leaf stopper |
| Aether Bloom | A white five-petalled flower with a green Aether core, petals lit from within |
| Bluefire Salve | A shallow stone dish of pale blue paste giving off cold blue vapour |

## Copilot Grid Prompts — Ready to Paste

Three batches covering all 24 items. Each is a single copy-paste block.

The grid instructions matter as much as the item descriptions: **no tile backgrounds, no frames, no banners, no labels, even spacing, pure white throughout.** That is what makes the sheet sliceable into individual transparent assets afterward.

---

### BATCH 1 — Common & Uncommon (7 items)

```
Create ONE image: a clean 3x3 grid of fantasy RPG inventory item icons.

CRITICAL LAYOUT RULES:
- Pure flat white background across the ENTIRE image
- NO background tiles, NO coloured squares behind items, NO frames,
  NO borders, NO banners, NO category headers, NO text or labels anywhere
- Each item fully isolated on white, evenly spaced, equal margins,
  consistent scale, not touching each other or the edges

SHARED STYLE for every item:
Painterly hand-illustrated game-asset style, three-quarter view, rich detail,
warm hammered gold trim, carved wood and living bark, woven vine, inset
glowing gems. Palette strictly bark brown, deep forest green, antique gold,
plus the accent colour noted per item. Faint green Aether energy tracing the
seams. No characters, no hands, no cast shadows.
Everything is GROWN, not forged — no steel, no plate armour, no wizard hats,
no animal pelts, no purple or pink gems.

THE 9 ITEMS (last two cells empty white):
1. Root Band — woven bark forearm cuff, three braided living roots, small
   green leaf buds where the strands cross, flat river stone at centre.
   Accent moss green.
2. Ember Ring — thick copper finger ring shaped like a curled flame, metal
   darkened from repeated forging, small orange ember glowing inside the
   curl. Accent ember orange.
3. Tideband — smooth temple circlet of driftwood and polished blue river
   stone, water endlessly beading along its underside. Accent pale blue.
4. Volt Brace — split ankle brace of dark wood banded with tarnished silver,
   the halves not quite touching, small yellow lightning arc leaping across
   the gap. Accent electric yellow.
5. Seedagon Charm — small carved wooden pendant of a sleeping seed sprite
   curled around a sprouting seed, worn smooth, soft green glow from within.
   Accent Aether green.
6. Greenhouse Gloves — worn canvas gardening gloves, soil-stained
   fingertips, bark patches sewn over the knuckles, tiny green shoots
   growing from the seams. Accent moss green.
7. Patrol Lantern — small hand lantern of bark and warped glass on a vine
   cord, containing a slowly rotating mote of green Aether light instead of
   a flame. Accent Aether green.
8. (leave empty white)
9. (leave empty white)
```

---

### BATCH 2 — Rare Accessories (8 items)

```
Create ONE image: a clean 3x3 grid of fantasy RPG inventory item icons.

CRITICAL LAYOUT RULES:
- Pure flat white background across the ENTIRE image
- NO background tiles, NO coloured squares behind items, NO frames,
  NO borders, NO banners, NO category headers, NO text or labels anywhere
- Each item fully isolated on white, evenly spaced, equal margins,
  consistent scale, not touching each other or the edges

SHARED STYLE for every item:
Painterly hand-illustrated game-asset style, three-quarter view, rich detail,
warm hammered gold trim, carved wood and living bark, woven vine, inset
glowing gems. Palette strictly bark brown, deep forest green, antique gold,
plus the accent colour noted per item. Faint green Aether energy tracing the
seams. No characters, no hands, no cast shadows.
Everything is GROWN, not forged — no steel, no plate armour, no wizard hats,
no animal pelts, no purple or pink gems.
These are RARE items — slightly more ornate and more Aether glow than common
gear, but the same materials and palette.

THE 9 ITEMS (last cell empty white):
1. Rootweave Armor — heavy chest piece of interwoven living roots and thick
   bark plating, moss in the crevices, gold banding at the shoulders, dense
   and immovable. Accent moss green.
2. Flameshod Boots — tall armoured boots in blackened gold, soles cracked
   and glowing orange like cooling forge metal, faint heat shimmer at the
   heels. Accent ember orange.
3. Tide Sigil — flat circular medallion of pale blue crystal in a driftwood
   frame, spiral wave carved into its face, water running UPWARD along the
   spiral against gravity. Accent pale blue.
4. Storm Crown — narrow open circlet of dark twisted branches with upward
   pointing tips, yellow lightning arcing continuously between the points.
   Accent electric yellow.
5. Aether Stone Pendant — raw uncut green Aether crystal wrapped in fine
   gold wire on a braided vine cord, glowing from deep inside as though lit
   by something far away. Accent Aether green.
6. Mageweave Cloak — heavy hooded cloak of deep forest green, gold
   leaf-shaped clasps at the throat, hem tattered into leaf shapes, faint
   green Aether motes drifting off the edges. Accent Aether green.
7. Fourfold Band — single wide ring divided into four seamless quarters:
   bark brown, ember orange, pale blue, electric yellow, each a different
   material, joined by thin gold seams. Accent all four.
8. Counter Wrap — layered vine and leather hand wraps bound tight across the
   knuckles, small green Aether stone knotted into the binding at the back
   of the wrist. Accent Aether green.
9. (leave empty white)
```

---

### BATCH 3 — Legendary & Healing Items (9 items)

```
Create ONE image: a clean 3x3 grid of fantasy RPG inventory item icons.

CRITICAL LAYOUT RULES:
- Pure flat white background across the ENTIRE image
- NO background tiles, NO coloured squares behind items, NO frames,
  NO borders, NO banners, NO category headers, NO text or labels anywhere
- Each item fully isolated on white, evenly spaced, equal margins,
  consistent scale, not touching each other or the edges

SHARED STYLE for every item:
Painterly hand-illustrated game-asset style, three-quarter view, rich detail,
warm hammered gold trim, carved wood and living bark, woven vine, inset
glowing gems. Palette strictly bark brown, deep forest green, antique gold,
plus the accent colour noted per item. Faint green Aether energy tracing the
seams. No characters, no hands, no cast shadows.
Everything is GROWN, not forged — no steel, no plate armour, no wizard hats,
no animal pelts, no purple or pink gems.
Items 2-9 are small consumables — simple, readable at thumbnail size.

THE 9 ITEMS:
1. Fifth Root Token — LEGENDARY, the most ornate item here. Heavy gold
   medallion shaped like a five-pointed root system radiating from a central
   seed. Four roots polished bright, the FIFTH left dark and unfinished.
   Deep green Aether pooling in the carved channels, warm inner light.
2. Dewleaf — a single broad green leaf cupped to hold one large faintly
   glowing bead of dew.
3. Rootbark Poultice — folded bundle of bark and moss tied with vine cord,
   damp and freshly packed.
4. Tidewater Vial — small round glass vial of luminous blue water, stoppered
   with carved driftwood.
5. Ember Root — gnarled root with its broken end glowing orange like a lit
   coal.
6. Sparksap — vial of thick golden sap with tiny yellow sparks suspended and
   drifting inside.
7. Seedagon Nectar — tiny acorn-shaped flask of warm amber nectar with a
   leaf stopper.
8. Aether Bloom — white five-petalled flower with a green Aether core,
   petals lit from within.
9. Bluefire Salve — shallow stone dish of pale blue paste giving off cold
   blue vapour.
```

---

### If the grid still comes back with tiles

Copilot sometimes ignores the layout rules and adds decorative backgrounds anyway. If that happens, the fastest fix is to add this line at the very top of the prompt:

```
Reference sheet on plain white paper, like a product catalogue page.
```

Framing it as a catalogue page rather than a game UI tends to suppress the inventory-slot styling.

---

## Production Notes

Once you have the images, drop them here and I'll process them exactly like the character art:

```
assets/accessories/<accessory-name>/<accessory-name>.webp
```

I'll standardize them to a uniform canvas, strip backgrounds to transparency, convert to WebP, wire them into this document, and rebuild the site.

**One difference from character art:** accessories should be **square (1:1)**, not the 900×1200 portrait used for characters and Sprites — items read better square in a table or card grid. I'll normalize them to **800×800**.


---

## Character Portrait Generation

Character art uses **900×1200 portrait** orientation (not the square 800×800 used for accessories). Each character portrait is a full-body depiction — no cropping at the waist, no bust-only framing. This is a TCG player-avatar portrait, not a D&D token.

### Shared Style Block for Characters

Paste this before each character prompt, unchanged, every time:

```
Single fantasy RPG character portrait, full-body, standing, centred, 900×1200.
Painterly hand-illustrated game-asset style with rich detail, warm saturated
colours, gentle rim lighting. Palette rooted in natural tones — bark brown,
deep forest green, moss, earth, amber — with one guild accent colour.
The character is made of living wood, bark, and Aether crystal — not flesh.
Faint green or guild-coloured Aether energy traces visible along seams,
joints, and cracks in their bark exterior.
Character on a plain flat parchment-warm background.
Full-length visible. No text, no watermark, no border, no frame.
```

Then append the character-specific line. Set accent colour per guild as noted below.

### Character Design Guidelines (World Consistency)

All ROOT Kingdom characters share these traits:
- **Material:** Living wood, bark, vine, and Aether crystal. No flesh, no fur, no scales, no metal armour (except small gold trim accents).
- **Eyes:** Glowing Aether — guild colour. Ground = moss green, Fire = ember orange, Water = pale blue, Energy = electric yellow. Mages have brighter, more active glow.
- **Proportions:** Humanoid, most between 5′ and 7′. Squires lean lanky, Warriors are broad-shouldered, Mages have elongated limbs and visible Aether crystal growths.
- **Clothing:** Woven vine, leaf-fabric, bark pauldrons, gold-thread sashes. No leather, no chainmail, no plate helmets.
- **Head:** Some characters have small branch-like antlers or a crown of leaves matching their guild. Bald is common — hair is rare in the ROOT Kingdom. When present, hair is made of fine root tendrils or moss.
- **Gender expression:** Present, but not through typical fantasy armour tropes. A character's bark texture, build, and posture signal identity.

### Per-Character Prompts

| Character | Guild | Accent Colour | Prompt Line |
|-----------|-------|-------------|-------------|
| Generic Ground Squire | Ground | Moss green | A young lanky bark-humanoid in woven vine tunic, moss-green Aether eyes, small leaf antlers, carrying a rootwood training staff, standing with unsure posture |
| Generic Ground Warrior | Ground | Moss green | Broad-shouldered bark-humanoid in bark pauldrons and gold-thread sash, moss-green Aether eyes, thick root legs braced, both fists raised in a ready stance |
| Generic Ground Mage | Ground | Moss green | Tall elongated bark-humanoid, moss-green Aether crystal jutting from one shoulder and both forearms, long vine robes, eyes glowing steady and bright |
| Generic Fire Squire | Fire | Ember orange | Wiry bark-humanoid with ember-flecked bark, orange Aether eyes, soot-smudged vine tunic, carrying a small wooden shield with a charcoal burn mark |
| Generic Fire Warrior | Fire | Ember orange | Heavy-set bark-humanoid, bark cracked like cooling lava exposing orange ember beneath, orange Aether eyes, gold armband on each wrist, crossed-arms stance |
| Generic Fire Mage | Fire | Ember orange | Lean bark-humanoid with ember-orange Aether crystal spines along both arms and down the back of the neck, orange Aether eyes blazing, one hand raised with embers drifting upward |
| Generic Water Squire | Water | Pale blue | Slender bark-humanoid with pale blue Aether eyes, moss between bark plates, driftwood club slung over one shoulder, standing with feet planted in a puddle |
| Generic Water Warrior | Water | Pale blue | Broad bark-humanoid with pale blue Aether eyes, shoulder-plates of smooth driftwood, small stream of water running continuously down one arm, relaxed neutral stance |
| Generic Water Mage | Water | Pale blue | Tall willowy bark-humanoid with pale blue Aether crystal woven into their chest like ribbing, blue eyes glowing softly, both hands at sides with water beading on the fingertips |
| Generic Energy Squire | Energy | Electric yellow | Lean fast-built bark-humanoid with electric-yellow Aether eyes, small sparks jumping between their bark plates, carrying a split-root shortsword in a relaxed grip |
| Generic Energy Warrior | Energy | Electric yellow | Compact muscular bark-humanoid with electric-yellow Aether eyes, yellow crystal shards embedded in both forearms, lightning-scarred bark, crouched combat-ready stance |
| Generic Energy Mage | Energy | Electric yellow | Spindly bark-humanoid with electric-yellow Aether crystal forming a half-crown around the head, yellow eyes flickering rapidly, both arms raised with arcs of yellow lightning linking them |

---

## Battle Arena Background Generation

Arena backgrounds are landscape-format (1920×1080) environmental illustrations. Each guild's Gate Battle Arena has a distinct biome that reflects the guild's Aether influence. These are **full-scene backgrounds** — no items, no characters, no UI elements.

### Shared Style Block for Arenas

```
Single wide fantasy RPG battle arena background environment, 1920×1080,
landscape format. No characters, no items, no UI. Painterly hand-illustrated
game-asset style with rich atmosphere, warm golden-hour natural lighting.
Everything is grown, not built — living wood, bark, vine, Aether crystal,
stone. Faint Aether glow suffusing the scene. No text, watermark, or border.
```

### Arena Backgrounds

| Arena | Biome | Prompt Line |
|-------|-------|-------------|
| **Ground Gate Arena** | Deep forest clearing | A wide forest clearing ringed by ancient gnarled trees with intertwined root walls, the floor a mosaic of packed earth and moss, green Aether motes drifting lazily through dappled sunlight filtering through the canopy |
| **Fire Gate Arena** | Volcanic ridge | A volcanic ridge arena with cracked obsidian floor plates and orange-glowing fissures, charcoal-black bark pillars at the edges, ember-orange Aether haze hovering low, distant smoke haze against a deep amber sky |
| **Water Gate Arena** | Shoreline lagoon | A shoreline lagoon arena with tidepools and natural driftwood barriers, pale blue Aether light reflecting off the water surface, mist rising from the warmer shallows, sky a soft grey-blue with low cloud |
| **Energy Gate Arena** | Storm-blasted highlands | A highland plateau arena with exposed root formations twisted by frequent lightning strikes, electric-yellow Aether crackling between the tallest root spires, sky dark grey-green with distant storm clouds, the air thick with static |
| **Training Arena (Interior)** | Indoor practice hall | An indoor practice hall of living bark walls and warm gold lanterns, worn smooth root-wood floor, ceiling open to the sky through a woven canopy, green Aether vein-lines running through the walls in slow pulses |
| **The Undergrowth** | Underground root cavern | A vast underground root cavern where the ceiling is a mass of tangled roots letting thin beams of light through, glowing fungi and Aether crystal clusters providing dim green-blue illumination, mist pooling at ankle height |

---

## Ability Icon Generation

Ability icons are small square assets (256×256) — one per named ability. Each icon represents a single action or effect in a clean, readable symbol format.

### Style Block for Ability Icons

```
Single fantasy RPG ability icon, square, 256×256, flat centred symbol on a
round or hexagonal wooden plaque background. Painterly hand-illustrated
game-asset style. Palette strictly bark brown, deep forest green, antique
gold, plus one accent colour per guild. Faint Aether energy glow around the
symbol edges. No text, no watermark, no character, no hand. Plain flat
parchment-warm background, item fully isolated.
```

### Icon Design Rules
- Each icon should be readable at 48×48 display size — bold silhouettes, minimal detail.
- Background plaque shape signals ability type: **circle** for offensive, **hexagon** for defensive, **rounded square** for support/heal, **diamond** for Aether/guild-specific.
- Aether crystal symbol inset in the centre represents the ability's element (moss green, ember orange, pale blue, electric yellow).



---

## Sprite Companion Portrait Generation

For characters who wish to commission a personal portrait of themselves alongside their Sprite companion, or for promotional art featuring a specific Sprite, use the guidelines below. These are **companion portraits** — the character and Sprite together in a single scene — not isolated Sprite icons.

### Shared Style Block for Sprite Portraits

```
Single fantasy RPG companion portrait, vertical, two characters — one
bark-humanoid Lady/Lord and one Sprite companion — standing together in a
natural forest or guild village setting. Painterly hand-illustrated
game-asset style with warm golden-hour natural lighting. Palette strictly
bark brown, deep forest green, antique gold, plus the accent colour of the
Sprite's guild. No text, no watermark, no border.
Everything is grown, not built — living wood, bark, vines, Aether crystal.
No forged steel, no plate helmets, no pointed wizard hats, no animal pelts.
```

### Per-Sprite Portrait Prompts

Each prompt uses the shared style block above plus the specific Sprite description from [06-sprites.md](06-sprites.md). The Lady/Lord character should be generic placeholder (no unique identifiers) unless a specific player commissioned the art. All sprites are named in the existing doc; add the following prompt lines after the style block:

| Sprite | Guild | Portrait Prompt Line |
|--------|-------|----------------------|
| **Bramblepuff** | Ground | A small round Sprite covered in dry moss and soft brown bristles, sitting on the shoulder of a Ground-guild Lady in bark armour, both looking toward a sunlit forest path, tiny root tendrils curling affectionately around the Lady's collar |
| **Fernad** | Ground | A gentle green Sprite in a flowing leafy cloak, holding a wooden staff, standing beside a Ground-guild Lord in weathered travelling gear, ferns and moss growing at their feet, teal Aether sparkles drifting from Fernad's fern crown |
| **Cinderclaw** | Fire | A compact lizard-like Sprite with dark cracked bark skin and glowing orange ember eyes, crouched at the feet of a Fire-guild Lady with a Sojourner Scar, orange Aether haze rising from the Sprite's spines in the evening light |
| **Kindle** | Fire | A tiny floating Sprite of glowing ember-orange Aether, hovering near a Fire-guild Lord's raised hand, leaving faint smoke trails in the air, both silhouetted against a volcanic sunset |
| **Rill** | Water | A small Sprite of dark smooth bark with pale blue Aether stripes, riding on the shoulder of a Water-guild Lady in driftwood-trimmed robes, a thin stream of water orbiting the Sprite's raised foreleg in a slow loop |
| **Driftfin** | Water | A sleek smooth-bark Sprite with translucent blue Aether fins and gills, half-submerged in a tidepool beside a Water-guild Lord with a Tide Sigil at his chest, pale blue Aether light reflecting off the water surface |
| **Zip** | Energy | A fast thin Sprite of dark bark with yellow Aether racing stripes along its limbs, mid-leap between two root pillars near an Energy-guild Lady, electric-yellow sparks trailing its motion in frozen arcs |
| **Static** | Energy | A spiky angular Sprite of dark cracked bark with yellow Aether crystal shards protruding from its joints, perched on a root outcrop beside an Energy-guild Lord, yellow lightning arcing between the Sprite's crystal shards and the nearest root spire |

### Portrait Composition Notes

- The Lady/Lord should occupy roughly 60% of the frame; the Sprite occupies 30%, with 10% environmental background.
- The Sprite should be at a natural scale relative to the character — shoulder-perch size for Bramblepuff, Rill, Zip; thigh-height for Cinderclaw, Static; waist-height for Fernad, Driftfin; hand-cupped for Kindle.
- Both character and Sprite should look at something off-frame (not at the viewer) unless the portrait is explicitly a character-card-style mugshot.
- Background should be a guild-biome setting (forest clearing / volcanic ridge / shoreline / storm highlands) consistent with the Sprite's guild.

---

## Guild Heraldry & Token Art

For badges, guild flags, scroll seals, and other small emblematic artwork needed by the Grand Counsel or individual guilds:

### Style Block for Heraldry

```
Single heraldic emblem, roundel format, flat centred design on a carved
wooden round plaque. Painterly hand-illustrated game-asset style. Palette
strictly bark brown, deep forest green, antique gold, plus one accent colour.
Faint Aether glow tracing the emblem's outline. No text, no border, no
watermark, no background tile. Plain flat warm parchment-coloured background,
emblem fully isolated.
```

### Guild Emblem Descriptions

| Guild | Accent Colour | Emblem Description |
|-------|---------------|--------------------|
| Ground Gate | Moss green | A thick tree root curling into a protective circle around a sprouting seed, set against a round bark plaque with moss at the lower edge |
| Fire Gate | Ember orange | A stylised flame shaped from a branching root with embers at its tips, centred on a circular charcoal-grey plaque with orange Aether glow behind it |
| Water Gate | Pale blue | A spiral wave carved as a continuous root tendril, set on a round driftwood-coloured plaque with pale blue Aether light pooling at the spiral's centre |
| Energy Gate | Electric yellow | Three jagged lightning bolts radiating from a central Aether crystal, set on a round dark-wood plaque with yellow Aether arcs linking the bolt tips |

### Grand Counsel Seal

For official Grand Counsel documents and proclamations:

> A five-pointed root system radiating from a central gold seed, all four guild colours inlaid into each root (moss green, ember orange, pale blue, electric yellow), the fifth root left dark and unfinished as per the Fifth Root tradition. Set on a deep green circular plaque with an Aether green glow behind the symbol. A thin gold border rings the edge.

### Production Size Guide

| Use Case | Resolution | Format |
|----------|-----------|--------|
| Guild Hall banner | 512×512 | PNG with transparent background |
| Scroll seal (digital doc) | 128×128 | PNG with transparent background |
| In-game badge (UI) | 64×64 | WEBP with transparent background |
| Physical cloth patch | Vector (SVG) supplied to printer | N/A |
