# Character Progression

## The Three Tiers

Characters evolve through three tiers. Each tier is a distinct identity — not just a number — representing a deeper bond with the ROOT Kingdom and the Aether. Root and Rooth change physically at each tier: they *grow*, visibly, like a tree putting on rings.

| Tier | Title | XP Required | Unlocks | Root Appearance | Rooth Appearance |
|------|-------|-------------|---------|----------------|-----------------|
| 1 | Squire | 0 (start) | Basic abilities, Sprite farming, Side Quests, basic training | Small wooden figure, leaf-top hair, green Aether veins, simple leaf-print clothes | *(art coming)* |
| 2 | Warrior | 1,000 XP | Tier-2 abilities, Gate Battles, Sprite leveling, Tier-2 Quests | Taller, angular hardwood features, golden plate armor over green, leaf crown, pointed ears | Full golden leaf-petal armor glowing at the chest, flowing green hair, yellow-green eyes, pointed ears |
| 3 | Mage | 5,000 XP | Aether channeling, Final Quests, Guild Counsel seat, gifting Aether/Sprites | Hooded green cloak over gold armor, glowing Aether sword, hood drawn, eyes gold | Pure gold armor and cloak, hood drawn, eyes blazing green, Aether sparks dissolving off the cloak edges |

> See [02-character-creation.md](02-character-creation.md) for full character art at each tier.

---

## Level-Up Ceremony

When a player reaches the XP threshold for the next tier, they must complete a **Level-Up Ceremony** — a brief ritual at the Tree of Life that is tracked on-chain.

### Ceremony Steps:
1. Travel to the Tree of Life node in the ROOT Kingdom (in-game action).
2. Roll **2d6** — this is the **Evolution Roll**.
3. Consult your guild's **Tier Ability Table** (see [05-abilities.md](05-abilities.md)) — the roll assigns you a new ability for that tier.
4. **Stat increases** are applied automatically (see table below).
5. A **Level-Up Card** is minted — a commemorative NFT snapshot of your character at that tier.

If a player already possesses the rolled ability (from training), they may re-roll **once**. On a second duplicate, they receive a **Mastery Token** for that ability instead (doubles its damage/effect).

---

## Stat Growth Per Tier

Stats increase at each tier based on guild.

### Squire → Warrior Stat Gains

| Stat | Ground | Fire | Water | Energy |
|------|--------|------|-------|--------|
| HP | +40 | +25 | +30 | +20 |
| SP | +10 | +15 | +20 | +25 |
| STR | +3 | +5 | +2 | +2 |
| DEF | +4 | +2 | +3 | +2 |
| WIS | +2 | +2 | +4 | +4 |
| AGI | +1 | +3 | +2 | +4 |

### Warrior → Mage Stat Gains

| Stat | Ground | Fire | Water | Energy |
|------|--------|------|-------|--------|
| HP | +60 | +40 | +50 | +35 |
| SP | +15 | +20 | +30 | +35 |
| STR | +4 | +7 | +3 | +3 |
| DEF | +6 | +3 | +5 | +3 |
| WIS | +5 | +4 | +7 | +8 |
| AGI | +2 | +4 | +3 | +6 |

---

## XP Sources

| Activity | XP Gained |
|----------|-----------|
| Completing a Side Quest | 20–50 XP |
| Completing a Tier Quest (Warrior) | 100–200 XP |
| Completing a Final Quest (Mage only) | 300–500 XP |
| Winning a Gate Battle | 30 XP |
| Losing a Gate Battle | 10 XP |
| Training a lower-tier player | 15 XP |
| Being trained by a higher-tier player | 10 XP |
| Daily Greenhouse Tending | 5 XP |
| Guild Patrol Duty | 8 XP |
| Sprite Evolution (first time) | 25 XP |

> **Squire Bonus:** When a Squire trains a Warrior or Mage, the higher-tier player receives a **Mentor Boost** — their XP from training is increased by 20% because training a newer player deepens mastery.

---

## Sprite Ownership and Tier

Sprite carrying capacity scales with tier:

| Tier | Max Sprites Carried |
|------|---------------------|
| Squire | 2 |
| Warrior | 5 |
| Mage | 10 |

Additional Sprites beyond the carry limit must remain in the Guild Greenhouse or be traded/gifted.
---

## Specialization Paths

At **Warrior tier**, a player chooses a **Specialization Path** — a focused combat and role identity within their guild. This choice shapes which of the guild's abilities come naturally and which role the player fills in Gate Battles and Raids.

Specializations are declared during the Warrior Level-Up Ceremony. A player may hold only one Path at a time. Path changes require a **Path Reroll** (see below).

### Ground Guild Paths

| Path | Philosophy | Playstyle | Signature Bonus |
|------|-----------|-----------|-----------------|
| **Ironclad** | The immovable wall | High DEF, shield abilities, absorb damage | DEF-based abilities deal +15% damage |
| **Oaken** | The enduring force | Balanced STR/DEF, self-healing, gradual pressure | Each turn in combat restores 3 HP passively |

### Fire Guild Paths

| Path | Philosophy | Playstyle | Signature Bonus |
|------|-----------|-----------|-----------------|
| **Blazeheart** | Burn everything now | Maximum burst damage, short cooldowns, low sustain | Critical Hit range expands from 6 to 5–6 |
| **Ashwalker** | Fire that outlasts | Burn/DoT focus, debuff stacking, extended pressure | Burn effects last +1 additional turn |

### Water Guild Paths

| Path | Philosophy | Playstyle | Signature Bonus |
|------|-----------|-----------|-----------------|
| **Foamrider** | Heal the front line | Primary healer, cleanse, ally buffs | Healing abilities restore +20% HP |
| **Deepwarden** | Control the battlefield | Debuffs, push/pull, terrain manipulation | Crowd-control effects last +1 additional turn |

### Energy Guild Paths

| Path | Philosophy | Playstyle | Signature Bonus |
|------|-----------|-----------|-----------------|
| **Thunderstep** | Hit fast, hit first | AGI stacking, first-strike bonus, mobility | +2 AGI for the first 3 turns of battle |
| **Lightweaver** | Connect everything | Buff allies, debuff enemies, team coordination | Buff/Debuff effects last +1 additional turn |

### Path Reroll

A player who wishes to change their specialization may do so by completing a **Specialization Trial** — a personal quest assigned by the Guild's High Sage:

- Trial difficulty scales with the player's current tier.
- Completion changes the player's Path immediately.
- The player cannot change Paths again for 30 days.
- **Token cost:** 200 $ROOT5, paid to the Guild Fund.


---

## Reputation & Renown

Alongside XP and tier progression, every character accumulates **Reputation** — a measure of their fame and standing within the ROOT Kingdom. Reputation does not affect combat power, stat growth, or character level. Instead, it unlocks cosmetic and social perks that reflect the character's renown across the guilds.

Reputation is earned through notable deeds, not routine grinding. The primary sources are:

| Action | Reputation Gained | Max per Week |
|--------|------------------|--------------|
| Win a Gate Battle | +15 | Unlimited |
| Participate in a successful Raid (any role) | +25 | 2 Raids |
| Complete a Side Quest with a faction outcome | +10–20 | Unlimited |
| Complete a Weekly Challenge | +10 | 3 Challenges |
| Complete an Enhancement Quest | +20 | Per quest |
| Win a Guild Championship | +50 | Once per event |
| Mentor another player (Skill Transfer session) | +5 | 10 sessions |
| Complete the Fifth Root Quest | +200 | Once |

### Renown Tiers

Reputation thresholds define a character's **Renown Tier**, which is displayed on their Character Card and in social interactions.

| Renown Tier | Reputation Required | Perk Unlocked |
|-------------|---------------------|---------------|
| **Unknown** | 0 | Default — no recognition |
| **Known** | 100 | Name appears in Guild Hall visitor log; NPCs remember meeting you |
| **Notable** | 300 | Guild Hall portrait slot unlocked (small). May be invited to minor Guild social events |
| **Esteemed** | 600 | Portrait slot upgraded to medium. NPCs from allied guilds offer friendlier dialogue options |
| **Famous** | 1,000 | Portrait slot upgraded to large. Guild broadcasts your victories in the village square. Title display gains a gold border on Character Card |
| **Renowned** | 1,500 | Your deeds are spoken of in other guild villages (NPC dialogue cross-pollination). Title display gains an Aether glow effect |
| **Legendary** | 2,500 | Full-body portrait slot in the Guild Hall. NPCs from rival guilds may offer respect dialogue. Fifth Root Token holders gain access to a private social channel |

### Reputation Decay

Reputation does not decay naturally. However, a character who has been inactive (no battles, quests, or training) for **30 consecutive real-world days** loses 25 Reputation per additional week of inactivity, down to a minimum of their next Renown Tier's threshold. This ensures active players remain the Kingdom's celebrated figures.

### Guild Reputation

In addition to personal Reputation, characters earn **Guild Reputation** — standing within their own guild. This is tracked separately and determines access to certain guild-only cosmetic perks:

- **Guild Hall private quarters** (Guild Rep 500+) — a small personal room with a bed, a chest, and a view of the village square
- **Guild-specific title prefix** (Guild Rep 800+) — e.g., *Ground's* [Ironclad], *Fire's* [Blazeheart]
- **Scroll Keeper access** (Guild Rep 1,000+) — the ability to request custom Enhancement Quests beyond the standard assignment rotation

Guild Reputation is earned at half the rate of personal Reputation (e.g. a Gate Battle win gives +15 personal and +7 Guild Rep).

> *"A warrior's strength is known in their arm. A hero's name is known at every gate."* — High Sage Mardon, Ground Guild

---

## Guild-Specific Training Academies

At **Mage tier**, players may join one of their guild's **Training Academies** — specialized study halls dedicated to perfecting the Path they chose at Warrior tier. These academies provide access to advanced techniques, mentorship from guild masters, and unique opportunities to master their specialization's full potential.

### Academy Requirements

To enroll in a Training Academy, a player must:

- Have achieved **Mage tier** in their chosen guild
- Possess the **Specialization Path** for their chosen academy
- Complete a **1,000 XP trial** involving advanced combat drills and mentorship sessions with the guild's High Sage
- Pay a **monthly fee** of 50  to the Guild Fund for academy maintenance

### Available Academies

| Academy | Guild | Specialization Focus | Unique Benefits |
|---------|-------|----------------------|-----------------|
| **Iron Academy** | Ground | Ironclad Path | Triple damage bonus when DEF > 20, gain temporary Stone Armor after using Shield abilities |
| **Forge Academy** | Fire | Blazeheart Path | Critical Hits apply Burn for 2 additional turns, burn damage scales with WIS |
| **Tide Academy** | Water | Foamdrid Path | Full healing on all status effect cleanses, regenerative water shield after healing allies |
| **Storm Academy** | Energy | Thunderstep Path | +1 to AGI for first 5 turns, gain first-strike bonus against enemies with AGI < 10 |

### Academy Training Benefits

Academy members receive:

- **Advanced Training Techniques** (once per week) that can be applied to any ability within their specialization
- **Guild Master Sessions** (monthly) — one-on-one training with the High Sage, including custom ability development
- **Academy Pass** — exclusive cosmetic title that appears before the player's name in all contexts
- **Resource Access** — free access to rare herbs, Aether crystals, and special materials at the Guild Greenhouse

### Academy Warfare Modifications

When participating in Gate Battles or Raids, Academy members may declare their **Academy Form**:

- **Ironclad Form** (Ground) — All damage calculations ignore the first 10 points of enemy DEF
- **Blazeheart Form** (Fire) — Critical Hit chance increases to 100% against burning enemies
- **Foamdrid Form** (Water) — All healing effects also restore 25% damage to the target's DEF
- **Thunderstep Form** (Energy) — Gain +3 AGI for the entire battle, and first-strike guarantee against any enemy

Academy Form lasts for exactly 5 battles or until the player's HP drops below 30%, whichever comes first.

> *The academy teaches you not just how to fight, but how to become the element.* — High Sage of the Storm Academy
