!!! note "Early technical draft (Feb 2026)"
    Kept for reference. Where it disagrees with the main chapters, the main chapters are current.

# Fifth Root: Game Architecture & World Design

Technical architecture and world structure documentation for Fifth Root.

## World Structure Overview

Fifth Root is built as a hybrid physical/virtual trading card game with RPG elements. The game world consists of 12 distinct areas organized around a central hub.

### World Layout

- **Central Hub**: Tree of Life - Where all players spawn
- **4 Guild Paths**: Fire (Red), Nature (Green), Water (Blue), Energy (White)
- **3 Levels per Guild**: Young (Level 1), Guardian (Level 2), Council (Level 3)
- **Total Areas**: 12 guild territories + 1 central hub = **13 total areas**
- **Aether Points**: Special zones in Level 3 territories

## Guild System

| Guild | Color | Element | Traits |
|-------|-------|---------|--------|
| **Fire Guild** | Red | Fire | Aggressive, fast-paced |
| **Nature Guild** | Green | Nature | Defensive, growth-focused |
| **Water Guild** | Blue | Water | Adaptive, healing |
| **Energy Guild** | White | Energy | Balanced, supportive |

## Backend Architecture

### Technology Stack

- **Frontend**: Rosebud.ai (exported to JavaScript)
- **Backend**: Node.js with Express.js
- **Real-time**: Socket.io for multiplayer
- **Database**: PostgreSQL for game state
- **Blockchain**: Solana with Anchor Framework
- **NFT Minting**: Metaplex
- **AI Service**: Claude API (Anthropic)

### Server Stack Diagram

```
[Player Browser]
       ↓
[Node.js + Express.js] ←→ [Socket.io Real-time]
       ↓
[PostgreSQL Database]
       ↓
[Solana RPC] ←→ [Anchor Programs] ←→ [Metaplex]
       ↓
[Claude API] (Ability Generation)
```

## Database Schema Overview

### Players Table

```sql
CREATE TABLE players (
  player_id UUID PRIMARY KEY,
  wallet_address VARCHAR(44),  -- Solana public key
  username VARCHAR(50),
  created_at TIMESTAMP,
  last_login TIMESTAMP
);
```

### Characters Table

```sql
CREATE TABLE characters (
  character_id UUID PRIMARY KEY,
  player_id UUID REFERENCES players,
  character_type VARCHAR(20),  -- 'Root' or 'Roothi'
  guild_path VARCHAR(20),      -- 'Fire', 'Nature', 'Water', 'Energy'
  level INT,                    -- 1, 2, or 3
  experience_points INT,
  aether_balance INT,
  ability_card_nft_address VARCHAR(44),  -- Solana token address
  current_position INT,
  created_at TIMESTAMP
);
```

### Sprites Table

```sql
CREATE TABLE sprites (
  sprite_id UUID PRIMARY KEY,
  character_id UUID REFERENCES characters,
  sprite_type VARCHAR(20),     -- 'Arbvorbis' or 'Seedagon'
  evolution_stage INT,         -- 1, 2, or 3
  health_points INT,
  attack_stat INT,
  defense_stat INT,
  speed_stat INT,
  sprite_nft_address VARCHAR(44),
  experience_points INT,
  created_at TIMESTAMP
);
```

### Seeds/Incubation Table

```sql
CREATE TABLE seeds_incubation (
  seed_id UUID PRIMARY KEY,
  character_id UUID REFERENCES characters,
  planted_at TIMESTAMP,
  hatch_at TIMESTAMP,
  care_score INT,              -- 0-100
  water_count INT,
  feed_count INT,
  health_checks INT,
  status VARCHAR(20)           -- 'planted', 'growing', 'hatching', 'hatched'
);
```

### Guild Territories Table

```sql
CREATE TABLE guild_territories (
  territory_id UUID PRIMARY KEY,
  guild_path VARCHAR(20),
  level INT,
  gate_health INT,
  market_inventory JSONB,
  active_defenders UUID[],
  created_at TIMESTAMP,
  last_raid TIMESTAMP
);
```

### Battles Table

```sql
CREATE TABLE battles (
  battle_id UUID PRIMARY KEY,
  attacker_character_id UUID REFERENCES characters,
  defender_character_id UUID REFERENCES characters,
  attacker_sprite_id UUID REFERENCES sprites,
  defender_sprite_id UUID REFERENCES sprites,
  battle_type VARCHAR(20),     -- 'training', 'raid', 'tournament'
  winner_id UUID,
  battle_log JSONB,
  xp_awarded INT,
  timestamp TIMESTAMP
);
```

## Blockchain Integration

### Smart Contract Structure

#### Character Creation Contract

- Records character creation on-chain
- Stores guild assignment and dice roll result
- Links to player wallet address
- Marks milestone for progression tracking

#### Ability Card NFT Contract

- Mints unique Aether Secret Ability card
- AI-generated ability stored in metadata
- Guild-specific attributes
- Tradeable on Solana marketplaces
- One card per character level-up (3 cards maximum per character)

#### Sprite NFT Contract

- Mints sprite after hatching
- Stats determined by care score (affects power level)
- Evolution updates metadata dynamically
- Tradeable/transferable between players
- Retains battle history and experience

#### Market Contract

- Handles guild market inventories
- Raid loot transfers (atomic transfers)
- Bartering mechanics between players
- Transaction fee system (small percentage to guild treasury)

## AI System Integration

### Ability Generation System

The AI system uses Claude API to generate unique abilities for each character based on their guild path and progression.

#### Input Parameters

- Guild path (Fire, Nature, Water, Energy)
- Character level (1-3)
- Character type (Root or Roothi)
- Dice roll result (2-12)
- Previous abilities (for evolution)
- Sprite type (Arbvorbis or Seedagon)
- Care score (affects power level)

#### Output Format

```json
{
  "ability_name": "Inferno Strike",
  "ability_description": "Unleash a burst of flame, dealing fire damage to a single enemy.",
  "power_level": 8,
  "element": "fire",
  "aether_cost": 25,
  "cooldown_turns": 2,
  "special_effects": [
    "30% chance to apply Burn status (deals 5 damage/turn for 3 turns)"
  ]
}
```

### Ability Generation Triggers

1. **Character Creation** - Initial ability based on guild selection
2. **Level 2 Evolution** - New Guardian-tier ability
3. **Level 3 Evolution** - Council-tier ability (most powerful)
4. **Sprite Hatching** - Unique sprite ability (generated once, tied to sprite)
5. **Sprite Evolution** - Enhanced sprite ability at stages 2 & 3

## Real-Time Multiplayer System

### Socket.io Event Architecture

```
Events:
├── Player Connection
│   ├── player:join
│   ├── player:spawn
│   └── player:disconnect
├── Guild Events
│   ├── guild:territory:update
│   ├── guild:raid:start
│   └── guild:raid:end
├── Battle Events
│   ├── battle:start
│   ├── battle:move
│   └── battle:end
├── Market Events
│   ├── market:item:buy
│   ├── market:item:sell
│   └── market:raid:loot
└── Chat Events
    ├── chat:message
    └── chat:announcement
```

### Real-Time Features

- **Guild territory updates** - Gate health, defender positions (updated per-second)
- **Raid events and capture-the-flag mechanics** - Live position tracking
- **Training session coordination** - Queue management and battle assignment
- **Tournament matchmaking and brackets** - Real-time bracket updates
- **Market transactions and loot distribution** - Atomic multi-player transfers
- **Guild chat and coordination** - Real-time messaging with guild channels

### Multiplayer Synchronization

All game state changes are:
1. Validated server-side
2. Applied to database
3. Broadcast to affected players via Socket.io
4. Client updates render immediately

## Security Considerations

### Wallet Authentication

- All blockchain actions require wallet signature verification
- Phantom/Solflare integration for key management
- Session tokens tied to wallet public key
- Rate limiting per wallet address

### Server-Side Validation

- All game actions validated before applying
- Dice rolls generated server-side (unhackable)
- Battle results determined server-side
- XP and rewards verified before minting

### Anti-Cheat Measures

- Server-side action validation
- Timestamp verification for time-based events
- Double-spend prevention for market transactions
- Battle log review for suspicious patterns

### Smart Contract Security

- Rate limiting on minting functions
- Owner/admin privileges for critical functions
- Escrow systems for raid loot distribution
- Audited smart contracts before mainnet deployment

## Performance Considerations

### Database Optimization

- Indexes on frequently-queried columns (player_id, character_id, guild_path)
- Connection pooling for high concurrency
- Read replicas for non-critical queries
- Caching layer for character stats

### WebSocket Optimization

- Message compression for large battle logs
- Event batching to reduce network overhead
- Selective broadcasting (only affected players receive updates)
- Graceful degradation if WebSocket connection drops

### Blockchain Optimization

- Batch minting for multiple NFTs
- Transaction bundling for gas efficiency
- Stateless smart contract design
- Caching of contract state (RPCs can be slow)

## Deployment Architecture

```
[Load Balancer (Nginx)]
         ↓
[Node.js Server Cluster (PM2)]
         ↓
[PostgreSQL (Primary + Read Replicas)]
         ↓
[Solana RPC Cluster]
```

---

This architecture provides a scalable foundation for Fifth Root's hybrid gameplay, combining the rapid development of Rosebud.ai with the robustness of a custom Solana backend.
