# Fifth Root: Character Creation & Onboarding

Player spawning and guild assignment process documentation.

## The Birth from the Tree of Life

Every player's journey begins at the center of the Fifth Root world, where the Tree of Life stands. Players are not created in the traditional sense—they are born, spawned from the very roots of this ancient tree, cut from its essence to begin their adventure.

## Spawning Animation

When a new player enters the game, they witness a cinematic spawning sequence:

1. Camera pans to the base of the Tree of Life
2. Roots begin to glow with golden energy (Aether)
3. A single root extends and begins to take shape
4. The root transforms into either Root or Roothi (player's choice)
5. Character opens their eyes, standing at the center

## Step 1: Character Selection

Before spawning is complete, the player must choose their form:

### Root (Young)

- Masculine-presenting wooden humanoid
- Tree crown hair (resembles a bushy green crown)
- Brown wooden skin with green vine patterns
- Sturdy, grounded appearance
- **Starting stats**: Higher defense, moderate attack
  - HP: 100
  - Attack: 15
  - Defense: 20
  - Speed: 10

### Roothi (Young)

- Feminine-presenting wooden humanoid
- Flowing leafy green hair
- Brown wooden skin with green vine patterns
- Graceful, agile appearance
- **Starting stats**: Higher speed, moderate defense
  - HP: 90
  - Attack: 18
  - Defense: 15
  - Speed: 17

## Step 2: The Four Portals

Once the character is chosen, they find themselves standing in a circular plaza at the base of the Tree of Life. Four glowing portals surround them, each pulsing with elemental energy:

### Red Portal - Fire Guild

- Crackling flames and intense heat
- Orange and red swirling energy
- Sound of roaring fire
- Gateway text: "The Path of Flame - For the bold and fierce"
- Traits: Aggressive, fast-paced combat style

### Green Portal - Nature Guild

- Vines and leaves growing around the edges
- Emerald green pulsing light
- Sound of rustling leaves and birdsong
- Gateway text: "The Path of Growth - For the patient and wise"
- Traits: Defensive, growth-focused progression

### Blue Portal - Water Guild

- Flowing water and gentle mist
- Deep blue and cyan rippling energy
- Sound of flowing streams
- Gateway text: "The Path of Flow - For the adaptive and fluid"
- Traits: Adaptive, healing-focused abilities

### White Portal - Energy Guild

- Crackling lightning and pure light
- Brilliant white and gold radiance
- Sound of electrical humming
- Gateway text: "The Path of Energy - For the balanced and powerful"
- Traits: Balanced, supportive abilities

## Step 3: Guild Path Selection

The player approaches one of the four portals. When they stand before their chosen portal, they see a message:

> "Roll the dice to determine your starting position on the path. Your journey begins now."

A prompt appears with a single button: **"Roll Dice"**

## Step 4: The Dice Roll

### Roll Mechanics

- Two six-sided dice appear and roll for 2 seconds
- Results can be 2-12 (snake eyes to double sixes)
- Result is stored in blockchain and database
- **Cannot be re-rolled** - this is your starting destiny
- Each dice roll result grants a unique ability (via AI generation)

### The Path Reveals Itself

After the dice roll completes, a glowing path appears extending from the portal. The path has 12 positions marked along it, corresponding to the possible dice roll results (2-12). The player's character automatically walks to their rolled position.

A message displays: 
> "You rolled [X]! Your journey begins at position [X] of the [Guild] Path."

### Dice Roll Probability Table

| Roll | Combinations | Probability | Rarity |
|------|--------------|-------------|--------|
| 2 | 1 | 2.8% | Legendary |
| 3 | 2 | 5.6% | Rare |
| 4 | 3 | 8.3% | Rare |
| 5 | 4 | 11.1% | Uncommon |
| 6 | 5 | 13.9% | Uncommon |
| 7 | 6 | 16.7% | Common |
| 8 | 5 | 13.9% | Uncommon |
| 9 | 4 | 11.1% | Uncommon |
| 10 | 3 | 8.3% | Rare |
| 11 | 2 | 5.6% | Rare |
| 12 | 1 | 2.8% | Legendary |

**Snake eyes (2) and boxcars (12) are legendary starting positions!**

## Step 5: Receiving the Aether Secret Ability

Once positioned on the path, the character passes through the portal and enters a mystical chamber. Here, they receive their unique Aether Secret Ability:

1. The Tree of Life's roots glow above the character
2. Golden Aether energy flows down
3. **AI generates a unique ability** based on:
   - Guild (Fire, Nature, Water, Energy)
   - Dice roll result (2-12)
   - Character type (Root or Roothi)
   - Starting stats influence
4. Ability card NFT is minted on Solana blockchain
5. Card appears in player's inventory with animation
6. Ability details are revealed with visual effects

### The Ability Card

The ability card displays:

- **Ability Name** - Guild-themed name
- **Ability Description** - What the ability does in battle
- **Power Level** - 1-10 scale
- **Aether Cost** - How much Aether to use in battle
- **Cooldown** - Turns until ability can be used again
- **Guild Emblem** - Visual identifier

### Example Ability Generation

**Guild**: Fire | **Dice Roll**: 7 | **Character**: Root

Output:
```json
{
  "ability_name": "Inferno Strike",
  "ability_description": "Unleash a burst of flame dealing fire damage",
  "power_level": 7,
  "aether_cost": 25,
  "cooldown": 2,
  "special_effects": ["30% chance to apply Burn status"]
}
```

## Step 6: Entering Level 1 Territory

With ability card in hand, the character steps through one final portal and emerges in their guild's Level 1 territory—the Sims-style RPG area where all Level 1, 2, and 3 players coexist.

They are greeted with a welcome message:

> "Welcome to the [Guild Name] Territory, young [Root/Roothi]. Your adventure begins here. Explore, train, care for seeds, and defend your guild's honor!"

### Tutorial Overlay

A brief tutorial highlights:

- **Training grounds** - where to gain XP
- **Market** - where to trade and restock
- **Plant Garden** - where to grow sprites
- **Guild Gate** - what you must defend
- **Other players in the territory** - your guildmates

## Onboarding Checklist

To help new players get started, an onboarding quest system guides them:

1. ✅ Visit the training grounds and complete a practice battle
2. ✅ Earn or purchase your first seed
3. ✅ Plant the seed in the garden
4. ✅ Perform your first care action (water/feed)
5. ✅ Visit the market and view available items
6. ✅ Meet three other guild members
7. ✅ Join a guild chat channel

### Onboarding Rewards

Upon completing the onboarding, players receive:

- **50 Aether** - Starting currency
- **1 Free Seed** - Ready to plant immediately
- **Onboarding Complete Badge** - Cosmetic achievement

## Character Data on Blockchain

After spawning, the following data is stored on-chain via the Character Creation Contract:

```json
{
  "character_id": "UUID",
  "player_wallet": "Solana public key",
  "character_type": "Root or Roothi",
  "guild_path": "Fire, Nature, Water, or Energy",
  "dice_roll": "2-12",
  "starting_position": "1-12",
  "ability_card_nft": "Solana token address",
  "timestamp": "creation timestamp"
}
```

## Guild-Specific Starting Bonuses

While all players start with the same base mechanics, each guild offers subtle thematic differences:

### Fire Guild Starting Bonuses
- Slightly higher starting Attack stat
- 10% XP boost in combat training
- Red-themed cosmetic items in starting inventory

### Nature Guild Starting Bonuses
- Slightly higher starting Defense stat
- 5% faster seed care progression
- Green-themed cosmetic items in starting inventory

### Water Guild Starting Bonuses
- Enhanced healing item effectiveness (+10%)
- 5% more Aether from battle rewards
- Blue-themed cosmetic items in starting inventory

### Energy Guild Starting Bonuses
- Balanced stat increase across the board
- 10% faster level progression
- White/gold-themed cosmetic items in starting inventory

---

**The character creation process is the player's first interaction with Fifth Root. It should be memorable, cinematic, and establish the tone for their entire journey.**
