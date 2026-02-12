# Fifth Root: Sprites & Abilities

Sprite evolution system and combat abilities documentation.

## Sprite Overview

Sprites are companion creatures that fight alongside players. They are hatched from seeds and can evolve through three stages based on care and battle experience. Sprites are minted as NFTs and can be traded or sold on Solana marketplaces.

## Sprite Types

Fifth Root features two distinct sprite evolution lines:

---

## Arbvorbis (Tree Sprite)

The defensive tree-based sprite line.

**Hatches when**: Seed care score ≥ 70

**Characteristics**: Strong defensive capabilities, growth-focused, nature-aligned

### Stage 1: Seedling Arbvorbis

**Appearance**
- Small sapling with glowing leaves
- Root structure visible
- Brown and green coloring
- Friendly, approachable design
- Size: Small (fits in hand)

**Stats**
- **HP**: 60
- **Attack**: 8
- **Defense**: 15
- **Speed**: 5
- **Total**: 88

**Abilities**
- **Root Grasp** (Primary Ability)
  - Entangles enemy, reduces speed
  - Power Level: 3
  - Aether Cost: 10
  - Cooldown: 1 turn
  - Effect: Enemy speed reduced by 50% for 2 turns

**NFT Metadata**
- Stage 1 designation
- Care score recorded (70-100)
- Owner's character ID
- Hatch timestamp
- Sprite type: Arbvorbis

---

### Stage 2: Guardian Arbvorbis

**Appearance**
- Medium-sized tree with thick bark armor
- Gnarled trunk with sturdy stance
- Enhanced coloring with gold accents
- Protective posture
- Size: Medium (shoulder height)

**Stats**
- **HP**: 150 (+90)
- **Attack**: 20 (+12)
- **Defense**: 35 (+20)
- **Speed**: 10 (+5)
- **Total**: 215 (+127)

**Abilities**
- **Root Grasp** (Inherited from Stage 1)
- **Bark Shield** (New Guardian Ability)
  - Creates protective barrier
  - Power Level: 6
  - Aether Cost: 20
  - Cooldown: 2 turns
  - Effect: Reduces all incoming damage by 30% for 3 turns

**Evolution Requirements**
- 500 sprite XP (gained through battles)
- Win 10 battles with sprite
- Owner character must be Level 1+
- Takes 5-7 days of regular battles

---

### Stage 3: Ancient Arbvorbis

**Appearance**
- Massive ancient tree with glowing runes
- Crystalline bark structure
- Elemental colors based on guild
- Towering presence
- Size: Large (towering overhead)

**Stats**
- **HP**: 350 (+200)
- **Attack**: 45 (+25)
- **Defense**: 70 (+35)
- **Speed**: 15 (+5)
- **Total**: 480 (+265)

**Abilities**
- **Root Grasp** (Original ability)
- **Bark Shield** (Guardian ability)
- **Nature's Wrath** (Ultimate Ability)
  - Summons thorny vines on battlefield
  - Power Level: 10
  - Aether Cost: 50
  - Cooldown: 4 turns
  - Effect: Area attack dealing 80 damage, applies thorns (DoT 10/turn for 3 turns)

**Evolution Requirements**
- 2000 sprite XP
- Win 50 battles with sprite
- Owner character must be Level 2+
- Complete special evolution quest
- Takes 10-14 days of intensive battles

---

## Seedagon (Dragon Seed Sprite)

The offensive dragon-based sprite line.

**Hatches when**: Seed care score < 70

**Characteristics**: Strong offensive capabilities, aggression-focused, primal energy

### Stage 1: Hatchling Seedagon

**Appearance**
- Small dragon with seed-shell wings
- Scaly baby dragon form
- Purple and green coloring
- Playful, energetic design
- Size: Small (size of fist)

**Stats**
- **HP**: 50
- **Attack**: 15
- **Defense**: 8
- **Speed**: 12
- **Total**: 85

**Abilities**
- **Seed Shot** (Primary Ability)
  - Fires seed projectiles
  - Power Level: 4
  - Aether Cost: 12
  - Cooldown: 1 turn
  - Effect: Single target physical attack, 25 damage + 20% chance critical hit

**NFT Metadata**
- Stage 1 designation
- Care score recorded (0-69)
- Owner's character ID
- Hatch timestamp
- Sprite type: Seedagon

---

### Stage 2: Warrior Seedagon

**Appearance**
- Larger dragon with scales and full wings
- Muscular build with extended wings
- Deep purple and gold coloring
- Battle-hardened appearance
- Size: Medium (dog-sized)

**Stats**
- **HP**: 130 (+80)
- **Attack**: 40 (+25)
- **Defense**: 20 (+12)
- **Speed**: 28 (+16)
- **Total**: 218 (+133)

**Abilities**
- **Seed Shot** (Inherited from Stage 1)
- **Dragon Breath** (New Warrior Ability)
  - Elemental breath attack
  - Power Level: 7
  - Aether Cost: 25
  - Cooldown: 2 turns
  - Element: Based on owner's guild
  - Effect: Area attack dealing 60 damage, 40% chance to apply status effect (Burn/Poison/Freeze/Shock)

**Evolution Requirements**
- 500 sprite XP
- Win 10 battles with sprite
- Owner character must be Level 1+
- Takes 5-7 days of regular battles

---

### Stage 3: Elder Seedagon

**Appearance**
- Massive dragon with crystalline scales
- Majestic wings with energy flows
- Brilliant guild-specific coloring
- Legendary, awe-inspiring presence
- Size: Huge (tower-sized)

**Stats**
- **HP**: 300 (+170)
- **Attack**: 80 (+40)
- **Defense**: 40 (+20)
- **Speed**: 45 (+17)
- **Total**: 465 (+247)

**Abilities**
- **Seed Shot** (Original ability)
- **Dragon Breath** (Warrior ability)
- **Primal Fury** (Ultimate Ability)
  - Devastating area attack
  - Power Level: 10
  - Aether Cost: 60
  - Cooldown: 4 turns
  - Effect: Area attack dealing 120 damage, applies Stun status (enemy skips next turn), 50% chance critical hit

**Evolution Requirements**
- 2000 sprite XP
- Win 50 battles with sprite
- Owner character must be Level 2+
- Complete special evolution quest
- Takes 10-14 days of intensive battles

---

## Sprite Evolution Requirements Summary

| Requirement | Stage 1→2 | Stage 2→3 |
|------------|----------|----------|
| Sprite XP | 500 | 2000 |
| Battle Wins | 10 | 50 |
| Character Level | Level 1+ | Level 2+ |
| Special Quest | None | Required |
| Timeline | 5-7 days | 10-14 days |

---

## AI-Generated Sprite Abilities

### Custom Ability Generation

Each sprite receives additional unique abilities based on:

- **Owner's guild path** - Fire, Nature, Water, or Energy
- **Sprite type** - Arbvorbis or Seedagon line
- **Care score during incubation** - Raw score affects power level
- **Evolution stage** - Powers up at each evolution

### Custom Ability System

At hatching, a custom ability is generated via Claude API:

**Input Variables**
```json
{
  "sprite_type": "Arbvorbis or Seedagon",
  "owner_guild": "Fire, Nature, Water, or Energy",
  "owner_level": 1-3,
  "care_score": 0-100,
  "dice_roll_modifier": 2-12 (from character creation),
  "evolution_stage": 1
}
```

**Output Ability**
```json
{
  "ability_name": "Nature's Blessing",
  "ability_description": "Heals all allies for 30 HP",
  "power_level": 5,
  "element": "nature",
  "aether_cost": 15,
  "cooldown": 3,
  "effect_type": "healing",
  "special_effects": [
    "Also increases Defense by 20% for 2 turns"
  ]
}
```

### Ability Uniqueness

- Each sprite's custom ability is unique
- Generated once at hatch, never changes
- Stored in NFT metadata permanently
- Becomes part of sprite's identity
- Contributes to sprite's trading value

---

## Sprite Battle Mechanics

### In-Battle Behavior

**Sprite Control**
- Sprite uses abilities automatically during battle
- Player can choose which ability to use each turn
- Player can boost sprite with Aether for enhanced attacks
- Smart AI chooses abilities based on battle situation

**Aether Boosting**
- Cost: 25-50 Aether per boost
- Effect: Next sprite attack deals 1.5x damage
- Can be stacked (multiple boosts increase multiplier)
- Strategic resource management

**Sprite Fainting**
- If sprite reaches 0 HP, it faints
- Player must choose:
  - **Run**: Escape battle, no XP or rewards
  - **Fight Alone**: Continue without sprite at disadvantage
    - Player attacks directly (lower damage)
    - Player takes more damage (no defense from sprite)
    - Victory grants reduced XP (50% normal)

### Sprite Recovery

**After Battle**
- Defeated sprites don't permanently die
- Sprites recover HP over time (1 HP per minute)
- Healing items restore HP instantly
- Can re-enter battle once healed

**Healing Items**
- Sprite Potion: Restores 50 HP
- Greater Sprite Potion: Restores 150 HP
- Full Sprite Restore: Restores all HP
- Available in Guild Market

### Multiple Sprites

**Owning Multiple Sprites**
- Players can hatch and own multiple sprites
- Only one sprite active in battle at a time
- Can switch active sprite between battles
- Strategy: build different sprite teams for different guilds

---

## Sprite Experience and Leveling

### Gaining Sprite XP

Sprites gain experience through:

| Activity | XP Gain |
|----------|---------|
| Win battle | 100-200 XP |
| Participate in battle (loss) | 50 XP |
| Training session | 20-50 XP |
| Sprite care | 5 XP (daily) |

### XP to Evolution

- **Stage 1→2**: 500 XP needed
- **Stage 2→3**: 2000 XP needed (resets counter)
- Progress tracked in sprite UI
- Visual progress bar shows evolution readiness

---

## Sprite NFT Metadata

Each sprite minted on Solana includes:

```json
{
  "name": "Seedling Arbvorbis #1",
  "description": "A defensive tree sprite from Fifth Root",
  "image": "IPFS_hash",
  "attributes": {
    "type": "Arbvorbis",
    "stage": 1,
    "hp": 60,
    "attack": 8,
    "defense": 15,
    "speed": 5,
    "care_score": 75,
    "owner_character_id": "UUID",
    "hatch_date": "2024-02-12T00:00:00Z",
    "custom_ability": {
      "name": "Seed Burst",
      "description": "Explodes with seeds, healing allies",
      "power_level": 4,
      "aether_cost": 12
    },
    "battle_record": {
      "total_battles": 10,
      "wins": 8,
      "losses": 2
    }
  }
}
```

---

## Sprite Trading

### Marketplace Sales

- Sprites can be listed on Solana NFT marketplaces
- Price determined by:
  - Evolution stage
  - Battle record
  - Custom ability power level
  - Rarity of hatch type
- Buyers gain full ownership of sprite NFT

### Trading Considerations

- High-level, evolved sprites command high prices
- Custom ability determines value
- Battle history affects prestige
- Rare hatches (low care score Arbvorbis) are valuable

---

## Guild-Specific Sprite Abilities

### Fire Guild Sprites

Custom abilities often include:
- Damage-over-time effects (Burn)
- Area damage spells
- Attack power boosts
- Fire element effects

### Nature Guild Sprites

Custom abilities often include:
- Healing effects
- Defense boosts
- Speed enhancements
- Growth multiplication effects

### Water Guild Sprites

Custom abilities often include:
- Healing and restoration
- Mana/Aether recovery
- Status effect cleansing
- Adaptive defense mechanics

### Energy Guild Sprites

Custom abilities often include:
- Balanced damage
- Critical hit boosts
- Speed enhancements
- Support/buff abilities

---

**Sprites are the heart of Fifth Root's gameplay loop. Each sprite is unique, valuable, and represents the player's commitment to the care and growth system.**
