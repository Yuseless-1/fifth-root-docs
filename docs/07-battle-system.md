# Battle System

## Overview

Battles in the ROOT Kingdom are structured, turn-based encounters that use dice rolls to determine turn order, damage variance, and critical hits. Every battle — whether a Gate Battle, a Raid, a training duel, or a quest fight — follows the same core rules.

---

## Battle Formats

| Format | Players | Location | Stakes |
|--------|---------|----------|--------|
| **Duel** | 1v1 | Training Arena or Gate Battle Arena | XP; Guild Points at gates |
| **Team Battle** | 2v2 or 3v3 | Gate Battle Arena, Raid | XP; Guild Points; Raid rights |
| **Raid** | Guild vs Guild (up to 5v5) | Opposing Guild Village | Flag capture; Sprite/XP penalty |
| **Quest Battle** | 1 player vs NPC | Quest zone | Quest rewards, XP |

---

## Pre-Battle: Turn Order Roll

Before every battle, **all participants** roll **1d20** to determine turn order.

- Highest roll acts **first**.
- In case of a tie between players, **compare AGI** — higher AGI breaks the tie.
- If AGI is also tied, re-roll 1d6 between the tied players only.

> **Energy Guild Passive:** Energy Guild players add their **AGI ÷ 5** (rounded down) as a bonus to their turn order roll. Example: AGI 15 → +3 to roll.

Turn order is set for the entire battle and does not change unless an ability modifies it (e.g., Volt Dash, Thunder Rush).

---

## Turn Structure

Each turn, a player chooses **one action**:

1. **Use an Ability** — select from your equipped ability set; pay SP cost
2. **Use a Signature Attack or Defense** — your innate Root/Rooth move; pay SP cost (does not use an ability slot — see [15-root-and-rooth-combat.md](15-root-and-rooth-combat.md))
3. **Declare Counter Stance** — Warrior tier and above only; forfeit your action to counter the next incoming attack (see [15-root-and-rooth-combat.md](15-root-and-rooth-combat.md))
4. **Deploy a Sprite** — place your Sprite on the field (costs your turn)
5. **Use a Healing Item** — consume a held item; no SP cost
6. **Defend** — take a defensive stance: incoming damage −30% until your next turn; no SP cost
7. **Cleanse** — remove one status effect from self or an adjacent ally (costs 10 SP, no ability slot needed)
8. **Flee** — attempt to exit a duel (70% success chance; if you flee a Gate Battle, your guild loses 5 Guild Points)

---

## Damage Calculation

**Base Damage Formula:**

```
Damage = (Ability Power + STR) × Elemental Modifier × Dice Roll Variance − Target DEF
```

- **Ability Power:** Listed in the ability table.
- **STR:** Attacker's STR stat (for Offense-type abilities).
- **WIS:** Used instead of STR for Aether-type abilities.
- **Elemental Modifier:** 1.25 if counter match, 0.80 if weak match, 1.0 if neutral.
- **Dice Roll Variance:** Roll **1d6** on every attack. Result maps to a damage modifier:

| 1d6 Roll | Modifier | Label |
|----------|----------|-------|
| 1 | 0.80 | Glance |
| 2–3 | 0.90 | Weak Hit |
| 4–5 | 1.00 | Solid Hit |
| 6 | 1.50 | Critical Hit |

- **Target DEF:** Subtracted after all multipliers. Minimum damage is always **1**.

> **Critical Hit (roll 6):** Deals 1.5× damage and ignores 50% of target's DEF. If a Mastery Token is active on the ability, a roll of 5 or 6 both count as Critical Hits.

---

## Example Turn (Step by Step)

> **Setup:** Kira (Fire/Warrior) attacks Toben (Ground/Warrior) using Volcano Spike.

1. **Turn Order Roll:** Kira rolled 14, Toben rolled 9. Kira goes first.
2. **Ability Selected:** Volcano Spike — SP Cost 30, Power 48.
3. **SP Check:** Kira has 65 SP → 65 − 30 = 35 SP remaining.
4. **Elemental Modifier:** Fire vs Ground = Fire counters Ground → ×1.25.
5. **Toben is Burned** (from previous turn): +15 bonus damage per Volcano Spike effect.
6. **Dice Roll Variance:** Kira rolls 1d6 → result: **6 (Critical Hit)**.
7. **Damage Calculation:**
   ```
   Base: (48 + 12 STR) = 60
   Critical: 60 × 1.50 = 90
   Elemental: 90 × 1.25 = 112.5
   Burned Bonus: +15 → 127.5
   Target DEF (Toben has 20 DEF; crit ignores 50% → 10 effective DEF)
   Final: 127.5 − 10 = 117.5 → 118 damage
   ```
8. Toben had 200 HP → now 82 HP.

---

## HP and Knockouts

When a player's HP reaches 0, they are **knocked out**:

- In a **Duel:** The battle ends immediately. Loser gains Knockdown XP (10 XP); winner gains Victory XP (30 XP).
- In a **Team Battle:** The knocked-out player is removed from the field. Their Sprites are recalled. Battle continues until one full team is knocked out.
- In a **Raid:** Knocked-out players are escorted out of the opposing village and may not re-enter that Raid.

Knocked-out players' HP is restored to **50%** after the battle ends. Full HP recovery requires resting at the Guild Village center or using an Aether Bloom item.

---

## SP Management

SP does not automatically recover during battle. Sources of in-battle SP recovery:

- **Tidal Recovery** (Water passive): +5 SP at turn start if SP > 50%
- **Fuel the Fire** (Fire ability): Convert HP to SP
- **Network Pulse** (Energy ability): All Energy allies +20 SP
- **Sap's Aether Gift** (Sap ability): +30 SP to all allies
- **Signal Boost** (Energy ability): Ally's next ability costs −5 SP

SP fully recovers after battle ends.

---

## Flee and Surrender

**Flee:** A player can attempt to flee on their turn. Roll 1d6:
- 1–2: Flee fails; lose your turn.
- 3–6: Flee succeeds; you exit the battle.

Fleeing a Gate Battle costs **5 Guild Points** (your guild's scoreboard).

**Surrender:** A player may type `/surrender` to end the battle without a dice roll. This counts as a loss with no penalties beyond the standard Knockdown XP payout to the winner.

---

## Sprite Battle Rules

When a Sprite is deployed:

- It acts on the **next turn** after deployment, in position determined by its SPD stat relative to other participants.
- It uses its Active Ability automatically (AI-controlled) or can be directed by the owner (in manual mode, if enabled in settings).
- Its Passive is always active from the moment it is deployed.
- If the owner is knocked out, all deployed Sprites are recalled immediately.
## Terrain Effects

Battles are not fought on empty ground. Every arena has terrain features that influence combat, shaped by the Guild Territory in which it sits and the history of battles fought there.

### General Terrain Rules

Terrain effects apply to all participants equally unless an ability or passive specifically overrides them. A Dungeon Master or the battle's auto-resolve system applies terrain effects at the start of the battle and updates them as the fight progresses.

- **Difficult Terrain** — Squares of difficult terrain (mud, rubble, ice) cost double movement to cross. Sprites and players entering difficult terrain have their SPD treated as −2 for turn order purposes that turn.
- **High Ground** — Elevated positions (rocky outcrops, gate platforms) grant the occupant +1 to their turn order roll and +10% damage with ranged or elevated attacks.
- **Cover** — Obstacles (pillars, walls, trees) provide half-cover: attacks targeting a character behind cover have a −10% hit chance. A character can move behind cover as a free action if it is adjacent.

### Arena-Specific Terrain

| Arena | Terrain Feature | Effect |
|-------|----------------|--------|
| **Ground — North Gate** | Rocky ridges | Half-cover squares along the northern wall. |
| **Ground — South Gate** | Muddy furrows | Difficult terrain in the south third of the arena. |
| **Fire — North Gate** | Scorched earth | No healing effects restore more than 10 HP per turn in the arena. |
| **Fire — South Gate** | Lava vents | Random lava vent (1d4 per turn): anyone on the vent square takes 8 fire damage. |
| **Water — North Gate** | Wet tiles | All movement costs are doubled; Slip risk on a 1d6 roll of 1 (lose next action). |
| **Water — South Gate** | Tidal pool | Standing in the pool restores 5 HP at the start of each turn. |
| **Energy — North Gate** | Conductive platforms | Water-based abilities deal +10% damage; Fire-based abilities deal −10% damage. |
| **Energy — South Gate** | Storm grid | Each turn, a 1d6 roll determines if lightning strikes a random square (6 = strike, 1–5 = safe). Struck characters take 12 damage and are **Stunned** for 1 turn. |

### Environmental Interaction

Some abilities can interact with terrain intentionally:

- **Earth abilities** can create or reinforce cover in Ground Territory battles.
- **Water abilities** can fill lava vents in Fire Territory (extinguishing them for 3 turns) or create temporary difficult terrain in non-Water arenas.
- **Energy abilities** can redirect lightning strikes in Energy Territory, choosing the target square instead of random.

Such interactions cost an additional action and are resolved through the standard turn structure.## Weather States

Beyond the static terrain of each arena, the ROOT Kingdom experiences shifting **weather** that adds dynamic conditions to every battle. Weather changes every **3 full turns** (one round for each participant counts as one turn). The Dungeon Master or auto-resolve system rolls on the territory's weather table at the start of battle and after every 3-turn interval.

### General Weather Table

These conditions can occur in any territory, though some are more likely in certain regions:

| Weather | Effect | Common In |
|---------|--------|-----------|
| **Clear** | No effect | All territories |
| **Overcast** | Turn order rolls have −1 penalty (poor visibility slows reactions) | All territories |
| **Light Rain** | +5% healing received; Fire abilities deal −10% damage | Water, Ground territories |
| **Fog** | All attacks have −10% hit chance; dodge +5% for all participants | Water, Ground territories |
| **Wind** | Ranged and AoE abilities deal +5% damage; movement costs +1 | Energy, Fire territories |
| **Ashfall** | All participants take 3 damage per turn (ignores DEF); Fire abilities deal +10% | Fire territory only |
| **Frostfall** | All participants take 2 cold damage per turn (ignores DEF). Fire abilities deal +15% damage. Water abilities deal −10% damage | Ground, Water territories |

### Territory-Specific Weather Tables

Each territory adds unique weather that only appears when battling within that guild's influence (any gate or arena within the territory's bounds).

| Weather | Territory | Effect |
|---------|-----------|--------|
| **Mist Haze** | Ground | Ground-based cover is doubled (half-cover becomes full cover); Water heal effects +10% |
| **Ember Gust** | Fire | Burning status effects spread to adjacent targets on hit; Wind effects enhanced |
| **Salt Spray** | Water | All participants gain **Soaked** for 1 turn at battle start; Energy abilities deal −10% damage |
| **Static Overcharge** | Energy | All Energy abilities cost −5 SP; non-Energy abilities have a 15% chance of causing the user to take 8 shock damage |

### Weather and Ability Interaction

Certain abilities can override or create weather:

- **Whirlpool** (Water Warrior): Creates **Salt Spray** in the target arena for 2 turns.
- **Stormcall** (Energy Mage): Summons a localized storm that acts as **Static Overcharge** for 3 turns.
- **Scorched Earth** (Fire Warrior): Creates **Ashfall** at the target's location for 2 turns.
- **Mist Veil** (Water Squire): Can be held as a free action to generate a single-square **Fog** cloud around the caster for 1 turn.

Using an ability to generate weather counts as the turn's action. Generated weather replaces the natural weather for its duration, after which the natural table resumes.

> *"The sky fights with us, or against us. Either way, know which."* — Ground Guild proverb
### Weather Duration & Tracking

Weather effects are tracked with an internal counter maintained by the Dungeon Master or auto-resolve system. Each weather effect has a **duration** listed in its description (e.g., 2 turns, 3 turns).

- Duration begins on the turn the weather takes effect and counts down each subsequent turn.
- If a new weather effect is generated while another is active, the new effect **replaces** the old one entirely — the old duration is discarded and the new countdown begins.
- Natural weather (rolled from the territory's weather table) and generated weather (from abilities) follow the same tracking rules.

When a weather effect expires, the territory's natural weather table is re-rolled at the next 3-turn interval.

### Cloudburst

**Cloudburst** (Water Mage) — SP Cost: 25, Power: 35

Summons a brief rainstorm that creates **Light Rain** and **Fog** simultaneously in the target arena for 2 turns. While Cloudburst is active:

- Fire abilities deal −15% damage.
- Healing received increases by 10%.
- All attacks have −10% hit chance.

Using Cloudburst counts as the turn's action. Generated weather replaces the natural weather for its duration, after which the natural table resumes.

> *"Even the sky needs a rest between storms."* — Water Squire saying


### Stormcall

**Stormcall** (Energy Mage) — SP Cost: 30, Power: 40

Summons a localized storm that creates **Static Overcharge** and **Cloudburst** simultaneously in the target arena for 3 turns. While Stormcall is active:

- All Energy abilities cost −10 SP.
- Non-Energy abilities have a 20% chance of causing the user to take 10 shock damage.
- Fire abilities deal −20% damage.
- Water abilities deal −15% damage.
- Healing received increases by 15%.
- All attacks have −10% hit chance.

Using Stormcall counts as the turn's action. Generated weather replaces the natural weather for its duration, after which the natural table resumes.

> *"A storm is only chaos until you learn its rhythm."* — Energy Mage saying

### Deep Fog

**Deep Fog** (Ground Territory) — A thick, ground-level fog that clings to the soil and muffles all sound.

| Weather | Territory | Effect |
|---------|-----------|--------|
| **Deep Fog** | Ground | All attacks have −15% hit chance; **Rooted** status effects last 1 extra turn; Water heal effects +20% |

> *"In the Deep Fog, even the roots forget which way is up."* — Ground Guild saying
