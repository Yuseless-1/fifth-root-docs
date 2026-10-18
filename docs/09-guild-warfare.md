# Guild Warfare

## Overview

Balance and order are the foundation of the ROOT Kingdom — but they must be earned and defended. Every guild competes for standing through Gate Battles and, when the balance tips far enough, has the right to **Raid** an opposing guild's village and attempt to capture their flag.

---

## Gate Battle Arenas

Each Guild Territory has a **North Gate** and a **South Gate**, each bordering an adjacent guild's territory. Entering a Gate Battle Arena is a declaration of challenge.

**Rules:**
- Any player can voluntarily enter a gate. Entering means you **must battle** the opposing guild's defender currently stationed there.
- If no defender is present, the gate is considered **undefended** — an automatic win for the challenger, awarding half the normal Guild Points.
- Defenders rotate on a voluntary sign-up schedule managed by the Guild Counsel.

**Formats at the Gate:**
- Default: **1v1 Duel**
- Players may challenge **2v2** if both teams agree and have the numbers

**Turn Order:** 1d20 roll per participant before every Gate Battle (see [07-battle-system.md](07-battle-system.md)).

---

## Guild Points (GP) Scoreboard

Every guild maintains a **Guild Points scoreboard** against each of its two neighboring guilds.

| Event | GP Change |
|-------|-----------|
| Gate Battle Win | +15 GP |
| Gate Battle Loss | −0 GP (no penalty for honest loss) |
| Undefended gate win (auto) | +7 GP |
| Patrol Duty completed | +2 GP |
| Player flees a Gate Battle | −5 GP |
| Raid Victory | +50 GP; resets opponent's GP to 0 |
| Raid Defeat | −20 GP |

The scoreboard is public and visible to all players. Guild Counsel members can also view a **24-hour trend** to anticipate raid thresholds.

---

## Raid Threshold

A guild earns the **right to raid** a neighboring guild when:

> **Their GP lead over that guild reaches 100 GP.**

*Example: Ground Guild has 200 GP against Fire Guild's 80 GP. Lead = 120. Ground may now raid Fire.*

Once a raid right is earned, the Guild Counsel must **vote to activate it** (see [10-counsel-structure.md](10-counsel-structure.md)). Raid rights expire after **48 hours** if not activated.

---

## The Raid

### Declaration

The raiding Guild Counsel declares the raid publicly. The target guild receives a **2-hour warning** notification before the raid begins. This is the preparation window.

### Raid Composition

- **Raiding Team:** 3–5 volunteers from the raiding guild (must be Warrior or Mage tier).
- **Defending Team:** 3–5 defenders from the target guild (must be Warrior or Mage tier).
- **Squires** may not participate directly in raids but can provide support (see below).

### Raid Map

The Raid takes place in the **target Guild's Village**. The map has three zones:

1. **Outer Gate** — Raiders must break through 1–2 defenders in a Team Battle.
2. **Village Center** — 1–2 more defenders hold the Training Arena.
3. **Flag Post** — Located at the Guild Hall. 1 Champion Defender guards it in a final 1v1 duel.

Each zone is fought sequentially. Raiders must win the Team Battle to advance.

### Squire Support Roles (Raid Support)

Squires cannot fight in raids but can:
- **Deliver a Healing Item** to one active raider or defender once per raid phase (their guild's members only).
- **Sound the Alarm** — alerting offline guild members via notification.
- **Tend the Greenhouse** — during a raid, a Squire can perform an emergency extra-tend to partially offset any Sprite care that will be missed.

### Winning the Raid

**Raiding guild wins** if they defeat all three zones and the Champion Defender.

**Consequences of Raid Victory:**

| Consequence | Target Guild |
|-------------|-------------|
| Flag is captured | Displayed in Raider guild's Hall of Trophies |
| XP penalty | All target guild members lose **25% of XP earned in the last 7 days** |
| Sprite penalty | All target guild members lose **50% of their current Sprite count** (NFTs are NOT destroyed — they go into a 72-hour escrow, then return) |
| Ransom option | Target guild can pay **500 $ROOT5** to recover flag and end penalties early |
| GP reset | Target guild's GP is set to 0 on that scoreboard |

> **Sprite NFT Safety:** Sprites in the 72-hour escrow period cannot be traded, gifted, or burned. They return automatically to owners' wallets when escrow ends or when the flag is ransomed.

**Defending guild wins** if they repel the raiders at any zone:

| Consequence | Raiding Guild |
|-------------|--------------|
| Raid fails | −20 GP |
| No XP or Sprite penalties on defenders | — |
| 48-hour raid cooldown | Raiding guild cannot declare another raid for 48 hours |

---

## Flag

Each guild's flag is a unique in-game asset stored in the Guild Hall:
- Displayed prominently in the village.
- Cosmetically represents the guild's identity.
- When captured, it disappears from the defender's hall and appears in the raider's Hall of Trophies (as a trophy NFT snapshot).
- The flag itself is always returned (either via ransom or after the 72-hour escrow).

---

## Peaceful Periods

The Grand Counsel (see [10-counsel-structure.md](10-counsel-structure.md)) can declare a **Peaceful Period** of up to 7 days, during which:
- Raids are suspended.
- Gate Battles still occur but earn no GP.
- All guilds gain a +10% XP bonus (encouraging training and growth rather than conflict).

Peaceful Periods require a unanimous Grand Counsel vote.
## Raid Aftermath

After a Raid concludes — whether it ends in victory, defeat, or the expiration of a raid window — the affected guilds enter a **Raid Aftermath** period that lasts 24 in-game hours. During this period, special rules apply to help the affected guilds recover and to prevent immediate re-escalation.

### Immediate Aftermath (24 Hours)

**For the defeated (raided) guild:**
- The Guild Fund is frozen for 24 hours — no deposits or withdrawals are permitted. This prevents griefing by rapid fund transfers during the vulnerability window.
- The Guild Greenhouse operates at **half efficiency** (50% incubation progress per day) — the Aether disruption from the raid lingers.
- All members receive a **Recovery Buff**: +10% XP from all activities. The guild is rebuilding, and every contribution matters.

**For the victorious (raiding) guild:**
- The raid right expires immediately after use. Even if the GP threshold is met again during the aftermath, a new raid cannot be declared for 48 hours (the standard cooldown).
- Captured flags are held in the raider's Hall of Trophies for 72 hours before the flag NFT is settled.
- All raiding participants receive a **Victory Bonus**: +25 XP each, regardless of individual performance.

### Flag Escrow

Captured flags are held in a special on-chain escrow:
- The flag NFT is transferred to the raider's guild wallet but marked as **escrowed**.
- During the 72-hour escrow, the defending guild can pay the **Flag Ransom** (500 $ROOT5, from the Guild Fund) to retrieve the flag early. This immediately ends the escrow and returns the flag.
- If no ransom is paid, the escrow expires and the flag NFT is permanently settled in the raider's Hall of Trophies as a trophy.
- The original flag NFT is always returned to the defending guild at the start of the next calendar year (January 1), regardless of who holds it.

### Post-Raid Assessment

The Guild Counsel of both the raiding and defending guilds should convene within 48 hours to review the raid:
- **What worked:** Document successful tactics, strong individual performances, and any exploits identified.
- **What failed:** Identify defensive gaps, communication failures, and coordination issues.
- **Aether restoration:** The defending guild's Counsel should schedule a collective tending ritual at Chad's roots to clear any Aether knots (see [01-world-lore.md](01-world-lore.md)).

This review is not mandatory but is considered best practice by established guilds.

> *"A raid lost is a lesson written. A raid won is a lesson earned."* — Ground Guild saying
## Raid Bounties

Beyond the flag and GP rewards, exceptional raids can earn a guild additional prestige through the **Bounty Board** — a public ledger maintained by the Grand Counsel that tracks the most memorable raid feats of each season.

### Bounty Tiers

Raids that meet certain criteria are elevated to bounty status, granting the participating raiders bonus XP on top of the standard Victory Bonus:

| Bounty Tier | Criteria | Reward |
|-------------|----------|--------|
| **Bronze Bounty** | Successful raid with 5+ participants | +50 XP per raider |
| **Silver Bounty** | Raid completed in under 30 minutes | +75 XP per raider |
| **Gold Bounty** | Raid against a guild holding a flag from a prior season | +100 XP per raider |

Bounty rewards are awarded after the 24-hour aftermath window closes and are logged on the Bounty Board in the raiding guild's village hall.

### Shield of the Gate

When a defender single-handedly repels a raid — dealing zero damage taken from the raiding party — their name is etched onto the **Shield of the Gate**, a permanent display in the defended guild's village. Shield holders receive a **+5% damage bonus** on all Gate Battles for the remainder of the season. Only one Shield of the Gate can be awarded per guild per season.

### Raid Standard

Each guild carries a **Raid Standard** — a small banner hung in their village hall that tracks the number of successful raids they have led. The guild with the most Raid Standards at the end of a season earns the title **Season's Champion**, granting all members a **+10 XP bonus** for the following month.

> *"The flag is taken once, but the legend echoes forever."* — Veteran raider saying

## Season Structure & Wartime Phases

The ROOT Kingdom's guild conflicts operate on a **seasonal cycle** — a recurring calendar that structures when wars begin, escalate, and wind down. Each season lasts **28 in-game days** and is divided into three phases:

### Warm-Up Phase (Days 1–7)

The first week of a season is dedicated to preparation. During this phase:
- Gate Battles are allowed but earn **reduced GP** (50% of normal).
- Guilds may declare **training alliances** — informal pacts where two guilds agree to spar without GP or flag stakes, using the same Raid composition rules but with no aftermath penalties.
- The Grand Counsel opens the **Season Outlook**, a public document outlining any scheduled Peaceful Periods, known conflicts, and the season's estimated GP rewards.

### Wartime Phase (Days 8–21)

The core of the season. All standard guild warfare rules apply:
- Raids may be declared freely (subject to GP thresholds and cooldowns).
- Gate Battles earn full GP.
- **Seasonal Events** may be announced by the Grand Counsel. These are special multi-guild conflicts with modified rules (e.g., a Blood Moon Raid where all captured flags earn double the standard XP).
- The **Bounty Board** is fully active.

### Cool-Down Phase (Days 22–28)

The season winds down. Key rules:
- No new raids may be declared (existing raids may conclude normally).
- Gate Battles still occur but earn only **25% GP**.
- The Grand Counsel tallies final Season's Champion standings.
- The **Hall of Trophies** is updated and all flag escrow periods resolve before the season ends.
- The next season begins immediately on Day 29 with a new Warm-Up Phase.

### Off-Season

The 7 days between seasons (Day 29–35 of the calendar) are considered **off-season**. During off-season:
- No Gate Battles or Raids occur.
## Guild War Memorials

The Guild War Memorials system honors fallen guild members and preserves their legacy for future generations, ensuring that every sacrifice made in defense of the ROOT Kingdom is remembered and respected.

### Memorial Categories

Guild War Memorials are organized into three tiers based on the significance of the fallen member's service and sacrifice:

1. **Guild Martyr** — Members who died defending a Gate or during a Raid, while actively engaged in guild warfare.
2. **Guardian of the Gate** — Members who died while defending a Gate under any circumstances, including during peaceful periods when guards were present.
3. **Warrior's Honor** — Members who died in any conflict directly related to guild warfare, including Field Battles and strategic skirmishes.

### Memorial Hall

Each guild maintains a **Memorial Hall** within their village — a quiet room adjacent to the Training Arena where names are inscribed on stone tablets. The Hall features:

- **Hall of Fallen Heroes** — Primary tablet wall listing all guild martyrs, with brief biographical notes and their final battle honor.
- **Gallery of Guardian Spirits** — Second wall dedicated to Gate defenders who gave their lives protecting their brothers and sisters.
- **Scroll of Honor** — Abundant scroll case containing commendations and personal items of honored warriors.

### Annual Memorial Day

The first day of every season, the surviving guild members gather at the Memorial Hall for **Memorial Day** ceremonies. The rituals include:

- **Morning Tending** — All present tend Chad's roots together to honor the life force that connects the living to their ancestors.
- **Name Recitation** — The current High Sage reads aloud the names of all fallen guild members from the previous season, ensuring that no sacrifice is forgotten.
- **Aether Offering** — Each attending member offers a small amount of their own Aether to the Tree of Life, symbolically passing on their life force to the next generation.
- **Sword Forging** — Young Squires forge ceremonial swords that will be displayed in the Memorial Hall, representing the continuation of the warrior tradition.

### Memorial Benefits

Active guild members who have tended the Memorial Hall regularly receive special benefits:

- **Memorial Tending Badge** — Wearable symbol granting +15% XP when tending the Memorial Hall for consecutive days (stacks to +30% at 7 days)
- **Hall Keeper Proficiency** — Access to exclusive guild hall crafting recipes (ceremonial swords, memorial tablets)
- **Legacy Voice** — Can speak at Guild Counsel meetings as an honorary representative for Memorial Hall matters (one use per season)
- **Aether Whisper** — Once per week, can call upon a brief echo of a fallen guild member (appears as spectral NPC for 10 minutes, offers historical lore and tactical advice)
- **Spirit of the Guard** — Passive: +5% damage against enemies who have been in previous seasons Memorial Halls
(recognizes the lingering Aether of fallen comrades)
- **Eternal Remembrance** — Access to the Memorial Hall outside of guild hours — a private meditation space for quiet contemplation and personal tending rituals.


### Memorial Rituals

Beyond the Annual Memorial Day, guilds perform regular rituals to honor their fallen:

- **Fallen Star Ceremony** — Held on the night of a new star appearance (in-game event), where guild members light **Aether Candles** that float to the sky, each bearing the name of a fallen comrade. The candles burn with the guild's elemental color and release stored Aether back to the Tree of Life.
- **Memory Stone Placement** — When a member falls in battle, their name is inscribed on a **Memory Stone** and placed in the Hall of Fallen Heroes. The stone absorbs a portion of the fallen member's Aether signature, allowing future generations to sense their presence when touching it.
- **Honor Guard Rotation** — Each season, two active members are selected as **Honor Guards** to stand watch at the Memorial Hall for one week, ensuring the space is always attended and the memories are never left unguarded.

### Veteran's Rest

The most honored fallen — those who achieved Mage tier and fell in the line of duty — are interred in the **Veteran's Rest**, a sacred grove behind each Memorial Hall. Here, their names are carved into the living roots of ancient trees that have witnessed centuries of guild history. These trees bear fruit once per year on Memorial Day, and the fruit is said to carry whispers of the fallen's wisdom.

> *The roots remember what the branches forget.* — Memorial Hall inscription
