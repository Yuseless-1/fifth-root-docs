# Fifth Root: Rosebud.ai Development Guide

How to Build Fifth Root Using AI-Powered Game Development

## Overview

This guide outlines the step-by-step process for building Fifth Root using Rosebud.ai's AI-assisted game development platform. The approach combines AI-generated code with your custom blockchain backend to create a hybrid physical/virtual trading card RPG.

## Why Rosebud.ai for Fifth Root

- **AI-powered code generation** - Build game mechanics through text prompts
- **RPG Maker template** - Perfect for turn-based combat and stat systems
- **Iterative development** - Test and refine systems quickly
- **Code visibility** - Export and modify for blockchain integration
- **Browser-based** - No downloads needed for players

## Development Architecture

### Phase 1: Core Gameplay in Rosebud

Build all game mechanics and visual elements using Rosebud's AI assistant:

- Character creation and guild selection
- Dice roll mechanics
- Sprite care system (Tamagotchi-style)
- Turn-based battle system
- Market and inventory UI
- Territory/gate defense
- Training and events

### Phase 2: Backend Integration

Export Rosebud code and connect to your Solana backend:

- Wallet authentication (Phantom/Solflare)
- NFT minting via Metaplex
- AI ability generation (Claude API)
- Real-time multiplayer (WebSocket)
- Game state synchronization

## Development Timeline

| Phase | Deliverables | Timeline |
|-------|--------------|----------|
| Phase 1: Prototype | Character creation, guild selection, dice mechanics, basic movement | 2-4 weeks |
| Phase 2: Sprites | Seed planting, care system, incubation, hatching mechanics | 1-2 weeks |
| Phase 3: Combat | Turn-based battle system, sprite battles, XP/leveling, evolution | 2-3 weeks |
| Phase 4: Guilds | Territory control, gate defense, raids, market/loot system | 2-3 weeks |
| Phase 5: Backend | Export code, wallet integration, NFT minting, AI abilities | 2-3 weeks |
| Phase 6: Launch | Testing, multiplayer, events, polish | 2-4 weeks |

## Prompting Strategy for Rosebud

### Best Practices

- Start with basic mechanics, iterate to add complexity
- Upload reference images for character consistency
- Test after each major addition
- Use specific numbers (dice rolls, stats, timers)
- Reference game mechanics by name (Tamagotchi, turn-based RPG)

### Example Prompt Sequences

#### 1. Character Creation Prompt

```
Create an isometric RPG character selection screen. Show two characters side by side:
Root (a wooden humanoid with tree crown hair, masculine features) and 
Roothi (a wooden humanoid with leafy flowing hair, feminine features). 
Both have brown wooden skin with green vine patterns. 
Add a 'Select Character' button under each. 

When clicked, move to the next screen showing 4 glowing portals arranged in a circle:
Red (Fire), Green (Nature), Blue (Water), White (Energy). 
Each portal should pulse with its respective color.
```

#### 2. Dice Roll System Prompt

```
When the player clicks a portal, roll 2 six-sided dice. 
Show the dice rolling animation for 2 seconds, then display the results. 
The combined dice roll (2-12) determines the player's starting position on a path within that guild. 

Add a visual path with 12 positions leading from the portal. 
Show the character moving to their rolled position. 
Display 'You rolled [X]! Your journey begins at position [X]' message.
```

#### 3. Sprite Care System Prompt

```
Create a seed planting system. Add a 'Plant Garden' area where players can plant a seed from their inventory. 

Once planted, show a seed icon in the ground. 
Add three care actions: Water (blue droplet button), Feed Aether (golden energy button), and Check Health (green heart button). 
Each care action increases a hidden care score. 
Show a health bar above the seed that fills with each care action. 

Add a timer showing 'Time until sprouting: XX hours'. 
When the timer reaches zero and care score is above 70, the seed hatches into Arbvorbis (tree-like sprite). 
If care score is below 70, it hatches into Seedagon (dragon-seed hybrid). 
Show hatching animation.
```

#### 4. Battle System Prompt

```
Create a turn-based battle system. At battle start, both player and opponent roll one die to determine 
initiative (highest goes first) and number of moves (die result = moves this turn). 

Show the battle UI with:
- Player sprite on left with health bar and Aether meter
- Opponent on right with health bar

Display available actions:
- Attack (sprite uses its ability)
- Defend (reduce incoming damage)
- Heal Sprite (restore sprite health using Aether)
- Boost Sprite (increase sprite's next attack using Aether)

Show damage numbers floating up when attacks hit. 
If sprite reaches 0 health, player must choose: Run (escape battle) or Fight Alone (continue without sprite at disadvantage). 

Winner gains XP shown as '+XX XP' floating message. 
Track XP in a progress bar under player portrait.
```

## Asset Requirements

### Character Sprites

- Root (Young) - front, back, left, right views
- Roothi (Young) - front, back, left, right views
- Root Guardian (Level 2) - armored version
- Roothi Guardian (Level 2) - armored version
- Multiple guild-colored outfit variants

### Sprite Creatures

- Seed (pre-hatch) sprite
- Arbvorbis - 3 evolution stages
- Seedagon - 3 evolution stages
- Attack animations for each sprite

### Environment Assets

- Portal effects (4 colors)
- Guild gates (4 designs)
- Tree of Life (center hub)
- Market buildings
- Training grounds
- Territory tiles (isometric)

## Technical Considerations

### Limitations to Plan For

- **No native blockchain support** - Requires custom integration
- **Limited multiplayer** - Real-time features need external server
- **Browser-based** - File size and performance constraints
- **Code export required** - For Solana wallet integration

## Success Metrics

- ✅ Playable prototype in 4-6 weeks
- ✅ Character consistency maintained across screens
- ✅ Smooth gameplay loop (create → care → battle → evolve)
- ✅ Exportable code for blockchain integration
- ✅ Community engagement and feedback incorporation

## Cost Breakdown

| Service | Monthly Cost | Notes |
|---------|--------------|-------|
| Rosebud.ai Pro | $20 | For export & monetization |
| Backend Server | $20-40 | DigitalOcean, Node.js + WebSocket |
| PostgreSQL | $15 | Game state storage |
| Claude API | $10-50 | AI ability generation |
| **Total** | **$65-125** | Scales with player base |

## Immediate Next Steps

1. Sign up for Rosebud.ai (free tier to start)
2. Upload character reference images (Root and Roothi)
3. Start with character selection prompt
4. Test and iterate on character movement
5. Add guild selection and dice roll mechanics
6. Set up ROOT5 DAO Solana backend in parallel
7. Join Rosebud Discord for community support

---

This guide provides the foundation for building Fifth Root using AI-assisted development. Refer to the accompanying game design documents for detailed specifications on characters, sprites, battles, and events.
