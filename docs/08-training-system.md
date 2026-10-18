# Training System

## Overview

The Training Arena at the center of each Guild Village is where players grow stronger — not just by fighting, but by learning from each other. Training is a cooperative system: higher-tier players teach skills, lower-tier players offer XP boosts in return, and both parties benefit.

---

## The Training Arena

Each Guild Village has one Training Arena. It is open at all times and can host up to **8 training sessions simultaneously**.

Sessions at the Training Arena are:
- Safe (no permanent damage; HP restores to 100% after each session)
- Opt-in (both players must agree to begin)
- Rewarding for both parties

---

## Types of Training

### 1. Skill Transfer

A higher-tier player can teach a skill they possess to a lower-tier player.

**Rules:**
- Teacher must be at least 1 tier above the student.
- Teacher must currently have the ability in their equipped set.
- The ability being taught must be the same tier or lower than the student's current tier.
- The session costs both players **30 minutes** of in-game time (or a real-time equivalent cooldown).
- The student receives the ability and adds it to their **Ability Scroll library** (not auto-equipped — they must slot it manually).

**Rewards:**
| Party | XP Reward |
|-------|-----------|
| Teacher (Warrior teaching Squire) | 15 XP |
| Teacher (Mage teaching Warrior) | 15 XP |
| Teacher (Mage teaching Squire) | 18 XP |
| Student | 10 XP |

**Squire Mentor Boost:** If a Squire trains a Warrior or Mage, the higher-tier player receives +20% XP from the interaction (because teaching a newer player sharpens mastery).

---

### 2. Sparring Match

A controlled 1v1 duel in the Training Arena. Same rules as a Duel (see [07-battle-system.md](07-battle-system.md)) but with no guild point consequences and reduced XP rewards.

**Dice throw at session start determines who goes first** (same 1d20 roll as all battles).

**Sparring Rewards:**

| Outcome | Winner XP | Loser XP |
|---------|-----------|---------|
| Squire vs Squire | 8 | 5 |
| Warrior vs Warrior | 10 | 7 |
| Mage vs Mage | 12 | 8 |
| Higher vs Lower tier | 6 | 10 (underdog bonus) |

> **Underdog Bonus:** A lower-tier player fighting a higher-tier player gains extra XP for the challenge, regardless of outcome.

---

### 3. Ability Practice

A player can practice a new or recently acquired ability against a **Training Dummy** — a non-combat target in the arena with fixed DEF of 5 and no HP limit.

Practice gives:
- **Dice variance experience**: The player rolls 1d6 on each hit; after 10 practice hits, they can review their roll distribution.
- **No XP reward** — this is purely mechanical familiarity.
- Ability cooldowns do not apply during practice.

---

### 4. Group Training (Mage-Led)

A Mage can lead a **Group Training Session** for up to 4 students of any tier in the same guild.

- The Mage selects a training theme: Offense, Defense, Heal, Buff/Debuff, or Aether.
- Each session lasts one in-game period.
- All students receive a themed ability from their guild's pool (Mage chooses which to teach).
- **Reward:** 25 XP to Mage, 15 XP to each student.
- **Limit:** A Mage can lead 2 Group Training sessions per day.

---

## Cross-Guild Training

Players from different guilds can train each other, but with restrictions:

- **Cross-guild sparring** is allowed in the Training Arena only — not Gate Battle arenas.
- **Skill Transfer** across guilds is **not permitted** — abilities are guild-specific.
- Cross-guild sparring earns **+5 bonus XP** for both parties (exposure to other fighting styles is valuable).

---

## Ability Scroll Library

Every ability a player learns goes into their **Ability Scroll Library** — a personal collection of all abilities they've ever acquired. The number a player can equip at once depends on tier: **4 slots at Squire, 6 at Warrior, 8 at Mage** (see [05-abilities.md](05-abilities.md)).

- Ability Scrolls not equipped are inactive in battle.
- Scrolls are tradeable cards. A player can trade a Scroll they no longer need to another player of the same guild.
- Scrolls of Mage-tier abilities **cannot** be traded to Squire or Warrior players — they appear grayed out until the recipient reaches the required tier.

---

## Training Cooldown

To prevent XP farming through repeated training loops:

- Each player can benefit from **Skill Transfer** as a student only **3 times per day**.
- Sparring has no daily limit.
- Mage-led Group Training can be attended by the same student only **once per day**.
- Cross-guild sparring has a separate limit of **2 sessions per day**.

---

## Training Arena Upgrades

Guilds can improve their Training Arena using Guild Fund resources (see [13-economy.md](13-economy.md)). Upgrades are permanent improvements purchased one time per guild and remain active as long as the guild's Guild Fund is solvent. The Counsel votes on whether to fund an upgrade — any Counsel Member or the Guild Master can propose it.

### Upgrade Tiers

| Tier | Cost (from Guild Fund) | Effect |
|------|----------------------|--------|
| **Basic Arena Expansion** | 500 $ROOT5 | Increases simultaneous session capacity from 8 to 12. Adds 2 Training Dummy stations so two players can practice abilities simultaneously. |
| **Aether-Conductive Flooring** | 1,200 $ROOT5 | All Skill Transfers in the upgraded arena grant +3 bonus XP to both teacher and student. The arena floor is inlaid with root channels that carry Aether from Chad's Grove, making skill transfer more efficient. |
| **Sparring Circle Enchantment** | 2,000 $ROOT5 | Sparring matches in the upgraded arena grant winners +2 XP and losers +3 XP (above the base rewards). Additionally, the Underdog Bonus for cross-tier sparring increases to 12 XP (from 10). |

### Unlock Requirements

- **Basic Arena Expansion:** Guild must have 15+ Active Members. Any guild can purchase this upgrade.
- **Aether-Conductive Flooring:** Requires Basic Arena Expansion first. Guild must have a Mage on the roster.
- **Sparring Circle Enchantment:** Requires both prior upgrades. Guild must have completed at least 1 Raid.

### Visual Changes

Each upgrade is visible in the village: new benches and practice rings appear around the Arena, root veins glow brighter on the floor tiles, and a small Aether crystal chandelier hangs above the Sparring Circle. These are world-dressing details — no separate art asset is needed beyond the existing arena tile.

---

## Aether Infusion Training (Mage-Led, Advanced)

A Mage who has led at least 10 Group Training sessions unlocks the ability to lead **Aether Infusion Training** — a deeper, more demanding session that temporarily attunes a student's combat abilities to Aether energy.

**Rules:**
- Requires a Mage who has the Aether Infusion Trainer title (earned after 10 Group Training sessions).
- Session lasts one full in-game period (double the length of a standard Group Training).
- The Mage spends 1 SP to initiate (their Aether kickstarts the infusion).
- Students must be Warrior tier or higher — Squire-tier players cannot yet channel Aether safely.
- Maximum 3 students per session.

**Effects (last for 3 battles or 7 days, whichever comes first):**
- Each infused student gains one of the following bonuses (Mage chooses at session start):
  - **Offensive Infusion:** +2 ATK for the duration
  - **Defensive Infusion:** +2 DEF for the duration
  - **Speed Infusion:** +1 AGI for the duration
- Infusion effects do not stack — a player can only hold one Aether Infusion at a time.
- Infusion ends immediately if the infused player takes part in a Raid (the chaos of raid combat disperses the concentrated Aether).

**Rewards:**
| Party | XP Reward |
|-------|-----------|
| Mage (session leader) | 35 XP |
| Each infused student | 20 XP |

**Limit:** A Mage can lead Aether Infusion Training once per week. A student can be infused at most twice per week (from any Mage).

## Seasonal Training Events

Three times per in-game year, the Training Arenas across all four guilds host **Seasonal Training Events** — structured, multi-day competitions that test players' abilities in themed formats. These events are organized by the Guild Counsel and open to all tiers.

### Event Structure

Each Seasonal Training Event spans **3 in-game days** and follows a bracket format:

- **Day 1 — Qualifying Rounds:** All participants enter a Swiss-style bracket. Matches are 1v1 sparring sessions (rules per [07-battle-system.md](07-battle-system.md)). Winning advances; losing earns consolation XP.
- **Day 2 — Team Trials:** Remaining players are seeded into teams of 3. Team battles test coordination and synergy (see [05-abilities.md](05-abilities.md) Ability Synergy section).
- **Day 3 — The Grand Session:** Finalists compete in a modified Group Training format — each finalist leads a training showcase for the audience, judged by Counsel members and Chad's Aether glow (Chad's pulse intensifies when a finalist uses an ability consistent with their guild's element).

### Seasonal Event Themes

| Season | Theme | Special Rule |
|--------|-------|--------------|
| **Roottide** | Defense-focused | All DEF buffs are +2 higher than listed |
| **Emberfest** | Offense-focused | All Offense abilities deal +10% damage |
| **Tidewake** | Healing-focused | All heal abilities restore +15% HP |
| **Insight Storm** | Intelligence-focused | All critical hits are +3 higher than listed |

### Rewards

| Placement | XP Reward | Item |
|-----------|-----------|------|
| Champion | 200 XP | Seasonal Champion title + Accessory (guild-themed) |
| Runner-up | 150 XP | Runner-up title |
| Semifinalist | 100 XP | 50 $ROOT5 |
| Qualifier | 50 XP | 25 $ROOT5 |

All participants receive a **Seasonal Spirit** badge on their Character Card for the following in-game year. This badge is cosmetic and does not affect gameplay.

> *"The arena tests not just your strength, but your spirit. Win or lose, you leave stronger."* — Training Arena maxim

---

## Training Gear & Equipment

All training sessions use standardized equipment designed to be safe, durable, and consistent across guilds. Training gear is provided free of charge by the guild at the start of each session and is stored in the Training Arena's equipment racks when not in use.

### Standard Training Kit

Every training session begins with the issuance of a **Standard Training Kit**, which includes:

| Item | Description | Used For |
|------|-------------|----------|
| **Practice Blade** | A wooden sword with a rounded tip and reinforced core, weighted to mimic the feel of a real weapon without dealing damage | Sparring matches, Skill Transfer drills |
| **Sparring Shield** | A lightweight shield reinforced with padded edges, designed to absorb impacts without injuring the wielder | Sparring matches, Group Training defense exercises |
| **Focus Stone** | A palm-sized crystal that resonates with the holder's Aether, providing tactile feedback during ability practice | Ability Practice, Aether Infusion Training |
| **Drill Pad** | A cushioned floor mat placed in the center of the Training Arena, absorbing impact from falls and ground-based techniques | All training session types |

### Equipment Rules

- Training gear is **non-transferable** — it cannot be taken from the arena, traded, or equipped outside of training sessions.
- Equipment is refreshed at the start of each session. Players who damage gear through negligence may be charged a small repair fee from the Guild Fund.
- **Higher-tier players** may bring their own training equipment to sessions, but it must pass a safety inspection by the Training Arena warden before use.
- Mage-led Group Training sessions may require additional equipment: **Aether Conduits** (glass rods that channel Aether for demonstration purposes) and **Resonance Crystals** (tuning forks that match the guild's elemental frequency).

### Equipment and the Training Arena Upgrades

The **Basic Arena Expansion** upgrade adds two additional **Training Dummy stations** — each station includes a reinforced Practice Blade rack and a padded Sparring Shield holder. The **Aether-Conductive Flooring** upgrade embeds Aether-sensitive runes into the Drill Pads, allowing them to glow brighter when a player's Aether output increases during a session — a visual indicator that helps Mages track their students' progress.

> *"The best weapon is the one that teaches you without cutting. The best armor is the one that catches you when you fall."* — Training Arena maxim

---

## Advanced Training Techniques

For players who have mastered the basics, the Training Arena offers specialized techniques to push their abilities further.

### Elemental Attunement Training

Mage-tier players can undergo **Elemental Attunement Training** to deepen their connection to their guild's element. This training is led by a Mage who has achieved at least 500 XP and has the **Elemental Master** title.

**Requirements:**
- Student must be Mage tier
- Student must have completed at least 10 Group Training sessions
- Training uses 2 SP from the student and 1 SP from the instructor

**Effects:**
- For 7 in-game days, the student's abilities of their guild's element deal **+5% damage**
- The student gains temporary access to one **elemental-exclusive ability** from their guild's pool
- The instructor receives 40 XP for sharing their elemental mastery

**Elemental-Exclusive Abilities:**
| Guild | Ability | Effect |
|-------|---------|--------|
| Ground | **Rootquake** | Deals damage to all enemies and reduces their DEF by 2 for 2 turns |
| Fire | **Inferno Surge** | Deals damage and applies a burn effect (3 damage/turn for 2 turns) |
| Water | **Tidal Wave** | Deals damage to all enemies and heals all allies for 10% of damage dealt |
| Energy | **Storm Charge** | Deals damage and charges all allies' next ability (+10% damage) |

**Limit:** A Mage can receive Elemental Attunement Training once per month. A Mage can instruct this training twice per week.

### Cross-Elemental Training

In a rare display of inter-guild cooperation, players from different guilds can participate in **Cross-Elemental Training** during Truce Days (see [03-guilds.md](03-guilds.md)). This training focuses on understanding and countering other elements.

**Rules:**
- Must be held during a Truce Day
- Requires at least one Mage from each participating guild
- Maximum 8 participants (2 from each guild)
- Focuses on counter-strategies and elemental weaknesses

**Rewards:**
- All participants receive 30 XP
- Participants gain **+15% damage** against the trained-against element for 3 in-game days
- Mages leading the session receive 50 XP

**Special Effect:** Cross-Elemental Training unlocks the **Elemental Scholar** title for participants, which can be displayed on their Character Card.

### Master-Apprentice Training

A time-honored tradition where a Mage takes on an apprentice (Squire or Warrior tier) for intensive one-on-one training. This relationship lasts for one full season (28 in-game days).

**Requirements:**
- Master must be Mage tier with at least 300 XP
- Apprentice must be Squire or Warrior tier
- Both must be from the same guild
- Only one apprentice per Master at a time

**Benefits:**
- **For the Apprentice:** Receives +20% XP from all training sessions with their Master, can request one **priority Skill Transfer** per week (jumps the queue if multiple students are waiting)
- **For the Master:** Receives +15 XP for every training session with their apprentice, gains the **Mentor** title which grants +1 to WIS while the apprenticeship is active
- **For Both:** Can participate in **Master-Apprentice Duels** — special sparring matches where the Master and Apprentice fight as a team against other Master-Apprentice pairs

**Master-Apprentice Duel Rewards:**
| Outcome | Master XP | Apprentice XP |
|---------|-----------|---------------|
| Victory | 25 | 35 |
| Defeat | 15 | 25 |

**Completion Bonus:** If the apprenticeship lasts the full season, both Master and Apprentice receive a **Seasoned Trainer** badge on their Character Card and 100 XP each.

> *A Master does not create a copy of themselves. A Master forges someone greater.* — Training Arena inscription
