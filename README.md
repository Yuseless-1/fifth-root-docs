# Fifth Root: Game Design Documentation

**The Hybrid Physical/Virtual Trading Card RPG on Solana**

This repository contains the complete game design documentation for Fifth Root, a next-generation trading card game that blends physical cards with blockchain technology.

## 📚 Documentation Structure

### Core Design
- **[Build Guide](./docs/01-build-guide.md)** - How to build Fifth Root using Rosebud.ai
- **[Game Architecture](./docs/02-game-architecture.md)** - Technical backend and world design
- **[Character System](./docs/05-character-evolution.md)** - Root and Roothi evolution system

### Gameplay Systems
- **[Onboarding & Character Creation](./docs/03-character-creation.md)** - Player spawning and guild assignment
- **[Level 1 Gameplay](./docs/04-level-1-gameplay.md)** - Core Sims-style RPG experience
- **[Sprites & Abilities](./docs/06-sprites-abilities.md)** - Companion creatures and combat abilities
- **[Events System](./docs/07-events-system.md)** - Tournaments, raids, and special events

## 🎮 Quick Start

**Fifth Root is organized around:**

1. **Character Creation** - Players spawn from the Tree of Life and choose guild
2. **Sprite Breeding** - Plant seeds, care for them, evolve powerful creatures
3. **Combat System** - Turn-based battles with sprites and abilities
4. **Guild Warfare** - Territory control, raids, and gate defense
5. **Progression** - Three player levels (Young → Guardian → Council)

## 🏗️ Technology Stack

- **Frontend**: Rosebud.ai (RPG Maker template, AI-assisted development)
- **Backend**: Node.js + Express.js with Socket.io for real-time multiplayer
- **Database**: PostgreSQL
- **Blockchain**: Solana with Anchor Framework + Metaplex
- **AI**: Claude API for unique ability generation

## 🎯 Development Timeline

| Phase | Deliverables | Timeline |
|-------|--------------|----------|
| Phase 1 | Character creation, guild selection, dice mechanics | 2-4 weeks |
| Phase 2 | Sprite system, care mechanics, incubation | 1-2 weeks |
| Phase 3 | Turn-based combat, XP/leveling, evolution | 2-3 weeks |
| Phase 4 | Guilds, territory control, raids, market | 2-3 weeks |
| Phase 5 | Backend integration, wallet, NFT minting | 2-3 weeks |
| Phase 6 | Testing, multiplayer, polish, launch | 2-4 weeks |

**Total Estimated Timeline: 11-19 weeks (~3-4 months)**

## 🌍 World Overview

Fifth Root's world consists of:
- **Central Hub**: Tree of Life (spawn point)
- **4 Guild Paths**: Fire, Nature, Water, Energy
- **3 Levels per Guild**: Level 1 (Young), Level 2 (Guardian), Level 3 (Council)
- **Total Areas**: 13 playable territories

### Guild System

| Guild | Color | Element | Trait |
|-------|-------|---------|-------|
| Fire | Red | Fire | Aggressive, fast-paced |
| Nature | Green | Nature | Defensive, growth-focused |
| Water | Blue | Water | Adaptive, healing |
| Energy | White | Energy | Balanced, supportive |

## 🎮 Core Gameplay Loop

1. **Spawn** at Tree of Life, choose guild, roll dice
2. **Plant** a seed and care for it (Tamagotchi-style)
3. **Battle** in training grounds to gain XP
4. **Evolve** your sprite and character
5. **Raid** enemy guilds or defend your territory
6. **Progress** through three levels with increasing responsibility

## 📊 Character Progression

### Root (Masculine Line)
- **Level 1**: Root (Young) - Base stats focused on defense
- **Level 2**: Root Guardian - Enhanced combat ability
- **Level 3**: Root Council - Majestic form with Aether aura

### Roothi (Feminine Line)
- **Level 1**: Roothi (Young) - Base stats focused on speed
- **Level 2**: Roothi Guardian - Enhanced agility
- **Level 3**: Roothi Council - Ethereal presence with nature effects

## 🐉 Sprite System

Each player hatches companion creatures called Sprites with two lines:

### Arbvorbis (Tree Sprite)
- **Stage 1**: Seedling Arbvorbis (defensive, weak)
- **Stage 2**: Guardian Arbvorbis (balanced)
- **Stage 3**: Ancient Arbvorbis (powerful defender)

### Seedagon (Dragon Sprite)
- **Stage 1**: Hatchling Seedagon (offensive, weak)
- **Stage 2**: Warrior Seedagon (powerful attacker)
- **Stage 3**: Elder Seedagon (devastating damage dealer)

Evolution type is determined by **care score during incubation**:
- Care Score ≥ 70: Arbvorbis (defensive)
- Care Score < 70: Seedagon (offensive)

## ⚔️ Combat System

Turn-based battles featuring:
- **Dice rolls** for initiative and turn count
- **Sprite abilities** (auto-attacking or player-boosted)
- **Aether system** for special moves
- **Running option** if sprite faints

## 🏰 Guild Systems

### Territory Control
- Each guild has a gate (health bar)
- Gate defense grants 200 XP per successful defense
- Raids use Capture-the-Flag mechanics

### Market
- Trading hub for items and resources
- Seeds, potions, Aether boosts, cosmetics
- Raided loot goes to winning guild

### Events
- **Guardian Tournaments** - Organized by Level 2 players
- **Guild Raids** - Require 60% guild vote
- **Council Cross-Guild Tournaments** - Prestigious inter-guild events

## 💾 Database Architecture

Key tables include:
- **Players** - Account data and wallet address
- **Characters** - Player progress and stats
- **Sprites** - Companion creatures and evolution state
- **Seeds_Incubation** - Growing sprites with care tracking
- **Guild_Territories** - Territory state and market inventory
- **Battles** - Combat logs and history

## 🔐 Blockchain Integration

### Smart Contracts

1. **Character Creation Contract** - Records on-chain guild assignment
2. **Ability Card NFT** - AI-generated unique abilities (minted per level)
3. **Sprite NFT** - Hatched sprites with stats and evolution
4. **Market Contract** - Raid loot transfers and trading

### NFT Minting
- **Ability Cards**: One per character level-up
- **Sprites**: Minted after hatching with dynamic stats
- **Special Cosmetics**: Guild-specific items and titles

## 🚀 Prompting Strategy for AI Development

The Rosebud.ai approach includes:

1. **Start simple** - Basic mechanics first, iterate to complexity
2. **Use reference images** - Upload character designs for consistency
3. **Test iteratively** - Validate each feature before adding next
4. **Be specific** - Use exact numbers (dice rolls, stat values, timers)
5. **Reference game mechanics** - Tamagotchi, turn-based RPG, etc.

### Example Prompt Categories
- Character creation and guild selection
- Dice roll mechanics
- Sprite care system (Tamagotchi-style)
- Turn-based battle system
- Territory and gate defense

See [Build Guide](./docs/01-build-guide.md) for detailed prompt examples.

## 💰 Operating Costs

| Service | Monthly Cost | Notes |
|---------|--------------|-------|
| Rosebud.ai Pro | $20 | Export & monetization |
| Backend Server | $20-40 | DigitalOcean, Node.js + WebSocket |
| PostgreSQL | $15 | Game state storage |
| Claude API | $10-50 | AI ability generation |
| **Total** | **$65-125** | Scales with player base |

## 📖 Documentation Roadmap

This documentation covers:
- ✅ High-level game design and mechanics
- ✅ Character progression and evolution
- ✅ Sprite breeding and battle systems
- ✅ Guild and territory systems
- ✅ Backend architecture overview
- ✅ Development timeline and prompting strategy
- 🚧 Detailed smart contract specifications (coming)
- 🚧 API endpoint documentation (coming)
- 🚧 Multiplayer event system details (coming)
- 🚧 Asset creation guidelines (coming)

## 🤝 Contributing

This documentation is maintained by the ROOT5 DAO team. For contributions or corrections, please create an issue or PR.

## 📄 License

Fifth Root is part of the ROOT5 DAO ecosystem on Solana.

---

**Ready to build?** Start with the [Build Guide](./docs/01-build-guide.md) to begin development using Rosebud.ai!
