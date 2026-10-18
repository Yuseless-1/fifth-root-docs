# Root & Rooth — Attacks, Defenses & Counterattacks

## Overview

Every ability in [05-abilities.md](05-abilities.md) is learned — rolled for at birth, earned through quests, or taught by another player. This document covers something different: the moves that belong to **Root and Rooth themselves**.

These are **Innate Moves**. They are not rolled for. They cannot be traded, taught, or lost. Every player has them from the moment they are born from the Tree of Life, and they grow stronger automatically at each tier.

> *Sprites are given their nature. Root and Rooth are given a choice — and a choice needs something to act with.*

**Innate Moves do not occupy ability slots.** A Squire with 4 active slots still has their Signature Attack, Signature Defense, and (from Warrior tier) their Counterattack available on top of those 4.

---

## The Three Innate Move Types

| Type | When Used | Cost | Purpose |
|------|-----------|------|---------|
| **Signature Attack** | Your turn | SP | Reliable damage that scales with tier — never runs out of relevance |
| **Signature Defense** | Your turn | SP | Protective stance unique to your character's nature |
| **Counterattack** | **Reactive** — triggers on the enemy's turn | Declared in advance | Punish an incoming attack instead of absorbing it |

---

## Design Principle — Equal but Opposite

Root and Rooth are equal in power. Their innate moves have **identical SP costs, identical cooldowns, and equivalent total value** — they differ only in *shape*.

| | Root | Rooth |
|--|------|-------|
| **Damage pattern** | Concentrated — single target, high spike | Distributed — multiple targets, sustained |
| **Defensive pattern** | Evasion and redirection — avoid the hit | Absorption and radiance — endure and reflect |
| **Counter pattern** | Precision punish — huge damage, narrow window | Area punish — smaller damage, wider window |
| **Battle identity** | The duelist | The anchor |

Neither is stronger. In a duel Root spikes harder; in a team battle or Raid Rooth contributes more. Pick the title you like — the game is balanced around both.

---

# ROOT — Innate Moves

![Root — Mage](https://cdn.root5dao.com/sites/fifth-root-tcg/assets/root/mage/root-mage.webp)

## Root's Signature Attacks

### Level 1 (Squire) — **Splinter Strike**
| | |
|--|--|
| **Type** | Offense |
| **SP** | 8 |
| **Power** | 16 |
| **Cooldown** | 0 |
| **Effect** | A sharp, quick strike with a hardened bark fist. If this is the first attack you make in a battle, it deals +5 bonus damage. |

*Root has no weapon yet. He has knuckles made of wood and the willingness to use them.*

---

### Level 2 (Warrior) — **Goldbreak**
| | |
|--|--|
| **Type** | Offense |
| **SP** | 20 |
| **Power** | 36 |
| **Cooldown** | 1 |
| **Effect** | An armored gauntlet strike. Ignores **20% of the target's DEF**. If the target is **Fortified**, **Stone Armor**, or has any active shield, this ability strips it before dealing damage. |

*Root's Warrior armor is not just protection — it is mass. Goldbreak is what happens when he decides to stop being polite about a defensive stance.*

---

### Level 3 (Mage) — **Aetherblade**
| | |
|--|--|
| **Type** | Aether |
| **SP** | 42 |
| **Power** | 70 |
| **Cooldown** | 3 |
| **Effect** | A single cut from the living Aether sword. Ignores **DEF entirely**. On a Critical Hit (1d6 = 6), applies **Weakened** for 3 turns and the cooldown resets to 0. |

*The blade is not metal. It is a length of the Tree of Life that agreed to be a sword. It cuts what it decides to cut.*

---

## Root's Signature Defenses

### Level 1 (Squire) — **Knothide**
| | |
|--|--|
| **Type** | Defense |
| **SP** | 10 |
| **Cooldown** | 2 |
| **Effect** | Root's bark thickens. Reduce incoming damage by **30%** until your next turn. If you are hit while Knothide is active, gain **+3 SP** (the impact rings the wood). |

---

### Level 2 (Warrior) — **Deadfall Step**
| | |
|--|--|
| **Type** | Defense |
| **SP** | 18 |
| **Cooldown** | 3 |
| **Effect** | Root goes still — completely still, like a tree that was always there. **60% chance to fully dodge** the next incoming attack. If the dodge succeeds, your next attack this battle deals **+15% damage**. |

*The most dangerous thing Root does is stop moving.*

---

### Level 3 (Mage) — **Hollow Cloak**
| | |
|--|--|
| **Type** | Aether |
| **SP** | 35 |
| **Cooldown** | 4 |
| **Effect** | The green cloak drinks the light around it. For 2 turns: incoming damage reduced by **40%**, you are immune to **Stunned**, and enemies cannot target you with AoE abilities while another valid target exists. |

---

# ROOTH — Innate Moves

![Rooth — Mage](https://cdn.root5dao.com/sites/fifth-root-tcg/assets/rooth/mage/rooth-mage.webp)

## Rooth's Signature Attacks

### Level 1 (Squire) — **Vinelash**
| | |
|--|--|
| **Type** | Offense |
| **SP** | 8 |
| **Power** | 13 |
| **Cooldown** | 0 |
| **Effect** | Rooth's vine hair snaps outward. Hits the target, then **chains to a second enemy for 6 damage** in team battles. In a duel, the second lash returns to the same target instead. |

*Rooth's hair is not decoration. It has opinions.*

---

### Level 2 (Warrior) — **Petalburst**
| | |
|--|--|
| **Type** | Offense |
| **SP** | 20 |
| **Power** | 30 |
| **Cooldown** | 1 |
| **Effect** | The golden leaf-plates of her armor flare outward in a ring. Hits **all enemies**. Each enemy struck gives Rooth **+2 HP** (healing scales with how many she hits). |

*Rooth's armor does not sit on her. It answers to her.*

---

### Level 3 (Mage) — **Aetherbloom**
| | |
|--|--|
| **Type** | Aether |
| **SP** | 42 |
| **Power** | 55 |
| **Cooldown** | 3 |
| **Effect** | The Aether pouring off her cloak detonates outward. Hits **all enemies**, ignoring **DEF entirely**, and **heals every ally for 20 HP** (including herself). On a Critical Hit, allies are also **Cleansed** of one status effect. |

*She does not aim it. She simply stops holding it in.*

---

## Rooth's Signature Defenses

### Level 1 (Squire) — **Rootstand**
| | |
|--|--|
| **Type** | Defense |
| **SP** | 10 |
| **Cooldown** | 2 |
| **Effect** | Rooth plants her feet and the ground answers. Reduce incoming damage by **30%** until your next turn. While Rootstand is active you cannot be pushed, pulled, or moved by any ability (**Tidal Push**, **Whirlpool**, knockback effects all fail). |

---

### Level 2 (Warrior) — **Lightward**
| | |
|--|--|
| **Type** | Defense |
| **SP** | 18 |
| **Cooldown** | 3 |
| **Effect** | The Aether light in her breastplate flares. Absorbs the next **40 damage**. Any attacker who strikes the shield is **Blinded** — AGI −4 for 1 turn. In team battles, one chosen ally also gains a 20-damage shield. |

---

### Level 3 (Mage) — **Radiant Veil**
| | |
|--|--|
| **Type** | Aether |
| **SP** | 35 |
| **Cooldown** | 4 |
| **Effect** | For 2 turns: incoming damage reduced by **40%**, Rooth is immune to **Stunned**, and **all allies within the veil heal 10 HP per turn**. Enemies attacking into the veil take **8 Aether damage** per hit. |

---

# The Counterattack System

## What Is a Counterattack?

A **Counterattack** is a reactive move. Instead of spending your turn attacking or defending, you spend it *waiting* — reading your opponent, holding your stance, and striking the moment they commit.

Counterattacks are unlocked at **Warrior tier**. Squires do not have them. Learning to counter is the mechanical marker of growing up in the ROOT Kingdom: a Squire reacts to what happened, a Warrior reacts to what is *about to*.

---

## Declaring a Counter Stance

On your turn, instead of taking any other action, declare **Counter Stance**:

1. **Pay the SP cost** of your Counterattack (listed below).
2. Your turn ends immediately. You take no other action.
3. Counter Stance remains active until the start of your next turn.
4. The **first** enemy attack that targets you while in Counter Stance triggers the **Counter Check**.

Counter Stance ends after one trigger — successful or not.

---

## The Counter Check (Dice Roll)

When an enemy attacks you while you are in Counter Stance, before damage is calculated, roll:

```
Counter Check = 1d20 + (your AGI ÷ 3, rounded down) + Tier Bonus
```

| Tier | Tier Bonus |
|------|-----------|
| Warrior | +2 |
| Mage | +4 |

Compare against the **Counter Threshold**:

| Situation | Threshold |
|-----------|-----------|
| Standard attack against you | **12** |
| Attacker has higher AGI than you | **15** |
| Attacker used an **Aether**-type ability | **17** |
| Attacker is **Stunned**, **Rooted**, or **Weakened** | **9** |

### Results

| Outcome | What Happens |
|---------|-------------|
| **Check ≥ Threshold — Counter Succeeds** | You take **50% damage** from the incoming attack, then immediately execute your Counterattack against the attacker. This does not use your next turn. |
| **Check < Threshold — Counter Fails** | You take **full damage**. Your SP is spent. Counter Stance ends. |
| **Natural 20 — Perfect Counter** | You take **no damage at all**, and your Counterattack deals **double damage**. |
| **Natural 1 — Overcommit** | You take **125% damage** and are **Stunned** for 1 turn. You read it completely wrong. |

> **Counters cannot be countered.** A Counterattack never triggers the opposing player's own Counter Stance. The chain stops at one.

---

## Root's Counterattacks

### Level 2 (Warrior) — **Splitwood Riposte**
| | |
|--|--|
| **SP** | 22 |
| **Counter Damage** | 45 |
| **Effect** | Root turns into the strike and drives an armored elbow through the opening. Deals damage and applies **Weakened** (STR −3, 3 turns) to the attacker. |

### Level 3 (Mage) — **The Quiet Answer**
| | |
|--|--|
| **SP** | 40 |
| **Counter Damage** | 85 |
| **Effect** | The Aetherblade moves before Root does. Ignores **DEF entirely**. If this Counterattack knocks the attacker out, Root's Counter Stance **immediately refreshes for free** and remains active for the next incoming attack. |

*Root does not say anything when he counters. That is the point.*

---

## Rooth's Counterattacks

### Level 2 (Warrior) — **Goldthorn Reversal**
| | |
|--|--|
| **SP** | 22 |
| **Counter Damage** | 34 |
| **Effect** | The leaf-plates of her armor snap outward into the attacker at contact. Deals damage to the attacker **and 15 damage to every other enemy** in a team battle. Rooth heals for **50% of the counter damage dealt**. |

### Level 3 (Mage) — **Consequence**
| | |
|--|--|
| **SP** | 40 |
| **Counter Damage** | 60 |
| **Effect** | The Aether she was holding back is released at the point of contact. Hits **all enemies**, ignoring **DEF entirely**. Every ally is healed **25 HP**. The original attacker is additionally **Stunned** for 1 turn. |

*She warned them. She warns everyone. They rarely listen.*

---

## Counter Interaction Rules

| Rule | Detail |
|------|--------|
| **One counter per stance** | Counter Stance triggers once, then ends — win or lose |
| **Sprites cannot counter** | Only Root and Rooth have Counterattacks; Sprites act normally |
| **Countering a Sprite** | You may counter a Sprite's attack; the Counterattack targets the Sprite, not its owner |
| **Counter vs. AoE** | If hit by an ability targeting all enemies, you may counter it, but the Counter Threshold increases by **+3** |
| **Counter vs. Counter** | Counterattacks never trigger an opposing Counter Stance |
| **Countering while Stunned** | Not possible — being Stunned cancels Counter Stance and refunds no SP |
| **Fleeing** | You cannot declare Counter Stance and attempt to Flee in the same turn |
| **Raid Champion Duels** | In the Flag Post duel of a Raid, both fighters may declare Counter Stance on the same turn — if so, neither triggers and both simply lose the turn |

---

## Worked Example — Countering in a Gate Battle

> **Setup:** Rooth (Water Guild, Mage, AGI 18) is in a Gate Battle against Kira (Fire Guild, Warrior, AGI 22).

1. **Rooth's turn:** She declares **Counter Stance**, paying 40 SP for *Consequence*. Her turn ends.
2. **Kira's turn:** Kira attacks with **Volcano Spike** (Power 48).
3. **Counter Check triggers.** Kira's AGI (22) is higher than Rooth's (18), so the Threshold is **15**.
4. Rooth rolls: `1d20 = 14`, plus AGI bonus (18 ÷ 3 = **+6**), plus Mage Tier Bonus (**+4**) = **24**.
5. **24 ≥ 15 — Counter Succeeds.**
6. Rooth takes **50% damage** from Volcano Spike instead of full.
7. *Consequence* fires immediately: **60 damage to Kira ignoring DEF**, all of Rooth's allies heal **25 HP**, and Kira is **Stunned** for 1 turn.
8. Kira loses her next turn. Rooth's turn comes around normally.

> Had Rooth rolled a natural 20, she would have taken **zero** damage and *Consequence* would have dealt **120**.

---

## When to Counter

Counter Stance costs you a full turn. It is a bet, not a default. Use it when:

- The opponent is **committed** — telegraphing a big cooldown ability
- You are **behind on HP** and need the 50% reduction plus a swing in one action
- The opponent is **Stunned, Rooted, or Weakened** — the Threshold drops to 9 and the odds are excellent
- You are the **Champion Defender** at a Flag Post and need to break a raider's momentum

Avoid Counter Stance when:

- The opponent is **faster and healthy** — Threshold 15 with no debuffs is a coin flip
- Facing an **Aether-type Mage** — Threshold 17 is a genuinely bad bet without high AGI
- Your **SP is low** — a failed counter spends the SP for nothing
---

## Innate Move Enhancement

Root and Rooth's innate moves are not static. Through dedicated training and specific personal quests, players can permanently upgrade their Signature Attacks, Signature Defenses, and Counterattacks at each tier.

### Enhancement Slots

| Tier | Enhancement Slots |
|------|-------------------|
| Squire | 1 (Attack or Defense) |
| Warrior | 2 (any two innate moves) |
| Mage | 3 (any three innate moves) |

Each tier's innate move can receive at most **one enhancement** for the life of the character. Splinter Strike (Squire), Goldbreak (Warrior), and Aetherblade (Mage) are enhanced independently.

### Enhancement Quests

Enhancement opportunities are assigned by the Guild's Scroll Keeper. A player may complete at most **2 Enhancement Quests per week** across all tiers.

#### Squire Enhancements

| Enhancement | Requirement | Effect |
|-------------|-------------|--------|
| **Hardened Splinter** | Win 3 Sparring Matches using Splinter Strike | *Splinter Strike*: Power +4; first-hit bonus increases from +5 to +7 |
| **Deep Knothide** | Absorb 300 total damage while Knothide is active | *Knothide*: Damage reduction improves from 30% to 35% |
| **Endless Vinelash** | Chain Vinelash to 5 different targets across battles | *Vinelash*: Second-hit damage increases from 6 to 8 |
| **Seeded Rootstand** | Resist 3 forced-movement effects while Rootstand is active | *Rootstand*: Damage reduction improves from 30% to 35% |

#### Warrior Enhancements

| Enhancement | Requirement | Effect |
|-------------|-------------|--------|
| **Gilded Goldbreak** | Knock out 3 enemies with Goldbreak | *Goldbreak*: DEF ignore increases from 20% to 30% |
| **Still Deadfall** | Dodge 5 attacks with Deadfall Step | *Deadfall Step*: Dodge chance improves from 60% to 70% |
| **Bright Petalburst** | Heal 150 HP total through Petalburst across battles | *Petalburst*: Healing per enemy increases from +2 to +3 HP |
| **Sheltering Lightward** | Shield an ally with Lightward 10 times | *Lightward*: Ally shield improves from 20 to 30 damage |
| **Wounding Riposte** | Successfully counter a Mage-tier attack | *Splitwood Riposte*: Weakened duration extends from 3 to 4 turns |
| **Venom Goldthorn** | Heal 200 HP through Goldthorn Reversal | *Goldthorn Reversal*: Heal increases from 50% to 65% of damage dealt |

#### Mage Enhancements

| Enhancement | Requirement | Effect |
|-------------|-------------|--------|
| **Enduring Aetherblade** | Land 10 Critical Hits with Aetherblade | *Aetherblade*: Critical Hit also restores 15 SP |
| **Vast Hollow Cloak** | Be hit by 25 attacks while Hollow Cloak is active | *Hollow Cloak*: Duration extends from 2 to 3 turns |
| **Overwhelming Aetherbloom** | Heal 500 HP to allies through Aetherbloom | *Aetherbloom*: Ally heal increases from 20 to 30 HP |
| **Burning Radiant Veil** | Deal 300 damage through Radiant Veil's reactive damage | *Radiant Veil*: Reactive damage increases from 8 to 12 per hit |
| **The Final Word** | Knock out 3 enemies with The Quiet Answer | *The Quiet Answer*: Also applies **Weakened** (3 turns) to any surviving target |
| **Unanswered Consequence** | Counter-attack a Raid Champion | *Consequence*: Stun duration increases from 1 to 2 turns |

### Enhancement Limit

A player can complete at most **2 Enhancement Quests per week**, regardless of tier. This ensures enhanced innate moves remain meaningful achievements rather than routine upgrades.


---

## Aether Echo — Transcendent Innate

When a character has filled **all available Enhancement Slots** for their current tier (see Enhancement Slots table — 1 slot for Squire, 2 for Warrior, 3 for Mage), and every enhanced move is fully quest-completed, they unlock a passive aura known as an **Aether Echo**. This is a permanent, irreversible bonus that activates automatically — no stance or toggle needed.

Aether Echoes are unique to each character and reflect the combination of enhancements they chose. There are no pre-defined Echo effects. Instead, the Echo synthesises the character's chosen enhancements into a single passive that feels like a natural extension of their combat identity.

### Echo Formation Rules

The Echo's effect is determined by a weighted formula based on which tier's moves were enhanced:

| Moves Enhanced | Echo Base Effect |
|----------------|------------------|
| Only Squire moves (1 slot filled) | **Rooted Presence** — The character's first move of each battle costs 2 less SP |
| Squire + Warrior (2 slots filled) | **Flowing Combat** — Switching between Attack and Defense stance costs 0 SP (normally 3 SP) |
| All three tiers (3 slots filled) | **Aether Harmony** — Once per battle, when HP drops below 25%, the character automatically recovers 20% of max HP and gains +1 to all stats for 3 turns. Does not stack |

### Echo Flavour Text

Each Aether Echo generates a unique flavour line displayed on the Character Card and whispered to the player on their first login after unlocking it:

- For a Ground-guardian who enhanced Hardened Splinter + Still Deadfall: *"The root does not flinch from the wind."*
- For a Fire-mage who enhanced Enduring Aetherblade + The Final Word: *"What burns out leaves no shadow."*
- For a Water-healer who enhanced Bright Petalburst + Sheltering Lightward: *"The tide does not ask permission to rise."*
- For an Energy-warrior who enhanced Wounding Riposte + Unanswered Consequence: *"The storm needs no second strike."*

Flavour text is generated by the Guild Scribe when the Echo unlocks and can be customised once (with the High Sage's approval) during a Character Card update.

### Echo Display

Once unlocked:
- The Character Card gains a faint animated Aether border in the character's guild colour.
- The Aether Echo's name (e.g., "Rooted Presence") appears as a subtitle on the Character Card beneath the character's title and Omen.
- In battle, the Echo effect triggers are visible as brief Aether particle bursts (green for Ground, orange for Fire, blue for Water, yellow for Energy).
- Echo effects are visible to allies in team battles — they can see the aura indicator on the character's portrait.

### Aether Echo & Path Reroll

If a character later changes their Specialization Path (see Path Reroll in 04-character-progression.md), the Aether Echo **remains active** — the Echo is tied to the character's innate moves, not to their guild role. However, if the character rerolls a Path after reaching Mage tier, they may request the Guild Scribe to recalculate one component of the Echo's flavour text. Mechanical effects are unaffected.

> *"The Tree's echo never fades. It only grows deeper."* — Fifth Root legend, chanted during Echo unlocking ceremonies
