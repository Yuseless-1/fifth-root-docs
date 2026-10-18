!!! note "Early technical draft (Feb 2026)"
    Kept for reference. Where it disagrees with the main chapters, the main chapters are current.

# Fifth Root: Events System

Guild events, tournaments, and raids documentation.

## Event Types Overview

Fifth Root features three main types of events that drive guild interaction and competition:

1. **Guardian Tournaments** - Organized by Level 2 players
2. **Guild Raids** - Guild-wide coordinated attacks
3. **Council Cross-Guild Tournaments** - Prestigious inter-guild events

---

## Guardian Tournaments

Organized and run by Level 2 Guardian players.

### Tournament Structure

**Format**: Single-elimination bracket

**Tournament Setup**
- Guardians can propose tournaments anytime
- Set entry requirements (level, guild, etc.)
- Choose guild-only or inter-guild
- Determine prize pool and rules
- Set tournament time

**Bracket Size**
- 4 participants (quickest: 2 rounds)
- 8 participants (standard: 3 rounds)
- 16 participants (large: 4 rounds)
- 32 participants (epic: 5 rounds)

### Tournament Rules (Customizable)

- **Level Restrictions**: Young only, or open to all
- **Sprite Rules**: With sprite, without sprite, or choice
- **Item Usage**: Allowed or banned
- **Healing Items**: Between rounds allowed/disallowed

### Tournament Progression

1. **Registration Phase** (2-24 hours)
   - Players register for tournament
   - Entry fee paid (optional, goes to prize pool)
   - Organizer can modify bracket up until start

2. **Tournament Start**
   - Bracket revealed to all participants
   - First round matchups begin
   - Matches happen sequentially or parallel

3. **Battle System**
   - Single 1v1 battle per matchup
   - Winner advances, loser eliminated
   - Best of 3 matches available (optional)
   - Matches conducted in real-time or async

4. **Tournament End**
   - Champion crowned
   - Results recorded permanently
   - NFT badges given to top 3

### Tournament Rewards

| Placement | XP | Aether | Items |
|-----------|----|----|-------|
| 1st Place | 1000 XP | 500 Aether | Rare Seed |
| 2nd Place | 500 XP | 250 Aether | Uncommon Seed |
| 3rd Place | 250 XP | 100 Aether | Healing Potion |
| Participation | 50 XP | 25 Aether | — |

### Tournament Cosmetics

**Badges for Top Finishers**
- Gold badge for 1st place
- Silver badge for 2nd place
- Bronze badge for 3rd place
- Tournament participation badge
- Badges display in player profile

**Special Titles**
- "[Tournament Name] Champion"
- Title displayed on character
- Persists until next tournament (unless retained)

---

## Guild Raids

Large-scale guild vs. guild warfare events.

### Raid Initiation Process

1. **Proposal Phase**
   - Guardian or Council member proposes raid
   - Guild members receive notification
   - Detailed raid proposal shown

2. **Voting Phase** (24 hours)
   - All guild members vote (yes/no)
   - Requires 60% approval to proceed
   - Council can override vote

3. **Challenge Phase**
   - Target guild is notified 24 hours before raid
   - They can prepare defenses
   - Defenders can organize counter-strategies

4. **Raid Window**
   - Organizer sets raid time (must be 48+ hours in future)
   - Raid duration: 1 hour active window
   - Can be extended if guilds agree
   - Real-time multiplayer event

### Raid Mechanics

**Format**: Capture the Flag

**Objective**: 
- Attackers must reach enemy guild gate and capture flag
- Defenders must prevent flag capture for 1 hour
- Multiple rounds of 1v1 battles

**Battle System**
- Attackers and defenders queue for battles
- 1v1 matchups determined by queue order
- Each win/loss affects gate health
- Gate health visible to both teams in real-time

**Gate Health System**
- Starts at 100 HP (full health)
- Decreases by 10 HP per attacker victory
- Each defender victory prevents 10 HP damage
- Reaches 0 HP = flag captured = attackers win
- Lasts 1 hour = defenders win

### Raid Timeline Example

```
Day 1: Raid proposed, voting starts
Day 2: Voting ends, if passed, challenge sent
Day 2 (late): Target guild prepares defenses
Day 3: Raid begins
  T+0:00: Raid window opens, first battles queue
  T+0:15: Multiple battles happening in parallel
  T+0:30: Gate health at 50%
  T+0:45: Defenders mounting comeback
  T+1:00: Raid window closes
  Result: Defenders held strong, raid fails
```

### Raid Outcomes

#### If Attackers Win

**Conditions**
- Gate health reaches 0 HP
- Flag is successfully captured
- Happens before 1-hour window closes

**Rewards for Attackers**
- Each participant: 500 XP
- Guild treasury: +500 Aether (from raid loot)
- Guild reputation: +200 points
- "Raid Victors" badge

**Impact on Defenders**
- All market inventory stolen by attackers
- Must rebuild market (takes time)
- Guild morale impact
- Option to launch counter-raid immediately

**Loot Distribution**
- All attacker-guild members split stolen goods
- Organizer gets 20% bonus share
- Distributed at end of raid
- Automated loot distribution system

#### If Defenders Win

**Conditions**
- 1-hour window closes with gate still active
- Gate health above 0 HP
- OR attackers run out of defenders

**Rewards for Defenders**
- Each participant: 300 XP
- Guild treasury: +300 Aether
- Guild reputation: +300 points (higher than attackers)
- "Gate Guardians" badge

**Gate Reinforcement**
- Gate gets temporary buff: +50% defense for 7 days
- Next raid against them is harder
- Stacks with multiple successful defenses

**Impact on Attackers**
- Raid fails, return with nothing
- Organizer loses prestige
- Can attempt counter-raid or revenge raid

---

## Council Cross-Guild Tournaments

Prestigious inter-guild championship events.

### Tournament Format

**Structure**: Open to all guilds

**Bracket System**
- Seeding based on player rankings
- Multiple brackets by level:
  - Young bracket (Level 1 players)
  - Guardian bracket (Level 2 players)
  - Council bracket (Level 3 players)

**Tournament Size**
- Each bracket: 8-32 players
- Single-elimination per bracket
- Grand Finals: Winner from each bracket competes
- Final Four: Top 2 from Young & Guardian, Council winner

### Prestige and Ranking

**Players are ranked by:**
- Battle win rate
- Tournament placements
- Guild reputation
- Raid victories
- Event participation

**Ranking Tiers**
- Bronze (0-100 rating)
- Silver (100-250 rating)
- Gold (250-400 rating)
- Platinum (400-600 rating)
- Diamond (600+ rating)

### Council Tournament Rewards

**1st Place (Champion)**
- 5000 XP
- 2000 Aether
- Legendary Sprite Egg (guaranteed rare hatch)
- Special Council-designed ability card (unique NFT)
- Title: "Champion of the Fifth Root"
- Permanent guild status boost

**2nd Place**
- 3000 XP
- 1000 Aether
- Rare Sprite Egg
- Special cosmetic items

**3rd Place**
- 2000 XP
- 750 Aether
- Uncommon Sprite Egg
- Special cosmetic items

**4th Place**
- 1500 XP
- 500 Aether
- Uncommon Sprite Egg

**All Participants**
- 500 XP base
- 100 Aether
- Participation badge
- Tournament cosmetics

### Championship Cosmetics

**Champion Cosmetics**
- Golden champion armor
- Golden aura effect
- "Champion" title (can display)
- Legendary sprite egg (guaranteed high-rarity hatch)
- Special ability card NFT (one-of-a-kind)

**Permanent Benefits**
- Champions get small XP multiplier (1.1x) for 1 month
- Can organize tournament at will
- Special market items available to champion

---

## Special Events

Limited-time seasonal and special events.

### Seasonal Events

**Spring Blossom Festival** (March)
- Nature guild celebration
- Plant and hatch special flower-themed sprites
- Bonus XP for sprite care (+50%)
- Limited edition seeds available
- 2-week duration

**Summer Solstice Challenge** (June)
- Energy guild event
- Double XP weekend
- Speed-based tournaments
- Limited edition light-themed cosmetics
- 2-week duration

**Autumn Fire Trials** (September)
- Fire guild competition
- Raid tournaments (guilds raid guilds)
- Bonus raid XP (+100%)
- Limited edition fire-themed items
- 2-week duration

**Winter Frost Games** (December)
- Water guild tournament
- Healing/support tournaments
- Bonus healing item effectiveness (+25%)
- Limited edition ice-themed cosmetics
- 2-week duration

### Limited-Time Events

**Rare Seed Hunt**
- Hidden seeds scattered in territories
- Players must explore to find
- Rare hatch types guaranteed
- Duration: 5 days
- Reward: First finder gets rare item

**Boss Raid**
- Super-powered enemy appears
- Guilds cooperate to defeat
- Requires coordinated efforts
- Victory grants guild-wide bonuses
- Duration: 1 week

**XP Boost Weekend**
- 2x XP for all activities
- Double rewards for battles
- Extra sprite care progression
- Usually announced Friday-Sunday
- Duration: 72 hours

### Event Participation

**Event Join**
- Simple opt-in system
- No prerequisites (usually open to all)
- Can join/leave any time
- Rewards accumulate

**Event Tracking**
- Real-time leaderboards
- Individual and guild standings
- Progress toward milestones
- Broadcast announcements

---

## Event Calendar

**Perpetual Schedule**

```
Weekly:
  - Guardian Tournaments (ongoing, organizer-initiated)
  - Daily quests and challenges
  - Raid windows (guild-initiated)

Monthly:
  - Council Cross-Guild Tournament (1st Sunday of month)
  - Guild Leaderboard reset

Seasonal:
  - Spring Blossom Festival (March)
  - Summer Solstice Challenge (June)
  - Autumn Fire Trials (September)
  - Winter Frost Games (December)

Special:
  - Boss Raid events (announced)
  - Rare seed hunts (varies)
  - XP boost weekends (varies)
```

---

## Event Rewards Summary

| Event | 1st Place | 2nd Place | 3rd Place | Participation |
|-------|-----------|-----------|-----------|----------------|
| Guardian Tournament | 1000 XP + Rare Seed | 500 XP + Uncommon | 250 XP + Potion | 50 XP |
| Guild Raid (Win) | 500 XP + Loot | — | — | — |
| Council Tournament | 5000 XP + Legend Item | 3000 XP + Rare Item | 2000 XP + Uncommon | 500 XP |
| Seasonal Events | Varies (2000+ XP) | Varies | Varies | 100-500 XP |

---

## Community Impact

### Guild Rankings

Guilds are ranked by:
- Total raid victories
- Tournament placings
- Member participation
- Guild reputation points
- Territory control duration

### Individual Rankings

Players are ranked by:
- Total XP (cumulative)
- Battle win rate
- Tournament placements
- Raid participation
- Event achievements

### Leaderboards

- **Global Leaderboard** - Top 100 players by XP
- **Guild Leaderboards** - Top players per guild
- **Battle Win Rate** - Competitive PvP ranking
- **Raid Victories** - Most successful raid leaders
- **Event Champions** - Tournament history

---

**Events drive community engagement, create opportunities for glory and rewards, and strengthen guild bonds through cooperative and competitive play.**
