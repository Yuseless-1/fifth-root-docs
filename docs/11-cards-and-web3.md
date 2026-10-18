# Cards & Web3

!!! warning "Under revision"
    This chapter is being updated. The game will run on **Solana** (Metaplex Core NFTs); Ethereum/Polygon references below are out of date. Any staking, yield or APY figures are design placeholders, **not offers or promises**. The rebalanced economy will replace them.


## Overview

The Fifth Root is a **hybrid trading card game** — every card has both a digital and physical form. The blockchain ensures provenance and ownership, while the physical cards bring the world into players' hands.

---

## Card Types

| Card Type | What It Represents | Mintable? |
|-----------|-------------------|-----------|
| **Character Card** | A player's Lady/Lord at their current tier | Yes — minted at each tier |
| **Sprite Card** | A minted Sprite companion | Yes — minted at sprouting; updated at evolution |
| **Ability Scroll Card** | A tradeable ability | Yes — minted when acquired, optional |
| **Accessory Card** | An equippable item | Yes — rare accessories are NFTs |
| **Level-Up Card** | Commemorative snapshot of a tier upgrade | Yes — auto-minted at tier ceremony |
| **Guild Points Card** | Proof of milestone GP contributions | Yes — milestone rewards |
| **Sap Card** | The legendary Sprite with living art | Yes — holographic NFT |

---

## Digital Cards

All digital cards live in the player's **in-game Card Gallery**, accessible from the dashboard.

### Digital Card Properties

Every card record contains:
- **Card ID** — unique on-chain identifier
- **Card Type** — one of the types above
- **Owner wallet** — linked web3 address
- **Metadata** — stats, abilities, guild, tier, hatch date, etc.
- **Art layer** — procedurally generated based on card type and player history
- **Rarity** — Common / Uncommon / Rare / Legendary
- **Mint date & block number** — permanent record

### Rarity Tiers

| Rarity | Color | How Obtained |
|--------|-------|-------------|
| Common | White border | Standard gameplay (quests, market) |
| Uncommon | Green border | Training milestones, uncommon quest drops |
| Rare | Blue border | Rare quest rewards, Warrior/Mage tier events |
| Legendary | Gold holographic border | Final Quests, Sap hatch, Grand Counsel appointment |

---

## Physical Cards

Physical cards are ordered through the **Fifth Root Card Print Service**, accessible in-game. Players select cards from their Gallery, place a print order, and receive physical cards by mail.

### Physical Card Features

| Feature | Details |
|---------|---------|
| **QR Code** | Unique code on the back of each card; scans to verify ownership on-chain |
| **Holographic Foil** | Applied to Rare and Legendary cards |
| **Sap Special Print** | All Sap cards printed with full holographic art on both front and back |
| **Watermark** | Guild symbol embossed in the card stock |
| **Edition Stamp** | Season/year printed; first-edition cards are marked "Genesis" |

### Physical ↔ Digital Bridge

Physical cards can be linked to their digital counterpart at any time:

1. Scan the QR code on the physical card using the Fifth Root app.
2. The app verifies the NFT on-chain and confirms the owner's wallet.
3. The physical card is now **linked** — it shows a live stat preview when scanned, reflecting current in-game values (useful for Sap cards that scale with XP).

**Physical Card in Play (Tabletop Mode):**  
The Fifth Root also supports a tabletop format using physical cards only. See the separate **Tabletop Rulebook** for physical play rules (draft in progress).

### Card Redemption

Physical cards can be redeemed for in-game items:
- **Common Physical Card** — redeems for a Sprite Seed when scanned
- **Uncommon Physical Card** — redeems for a healing item bundle
- **Rare Physical Card** — redeems for a random Rare Accessory
- **Legendary Physical Card** — redeems for a Fifth Root Token (see accessories)

Each physical card can be redeemed **once**. After redemption, the card's QR code is still valid for identity verification but no longer grants in-game items.

---

## Blockchain & NFT Details

### Supported Networks

At launch, the game supports player wallet connections on:
- **Ethereum Mainnet** — for high-value assets (Sap, Legendary cards)
- **Polygon** — for everyday Sprite minting and card trading (lower gas fees)
- **Player's choice** — at hatching, the player selects which supported network to mint to

### What Lives On-Chain

| Asset | On-Chain? | Notes |
|-------|-----------|-------|
| Sprite (all types) | Yes | Minted at sprouting; burned and re-minted at evolution |
| Character Card | Yes | Minted at each tier; previous tier card is not burned |
| Ability Scrolls | Optional | Player chooses whether to mint each Scroll |
| Accessories (Rare+) | Yes | Common accessories are off-chain |
| Level-Up Cards | Yes | Auto-minted; purely commemorative |
| GP Milestone Cards | Yes | On-chain proof of contribution |
| In-game currency (Sprites) | Hybrid | Tracked in-game; major transactions can be settled on-chain |

### Trading

All NFT cards can be traded peer-to-peer:
- In-game via the **Guild Market** or **Direct Trade** interface
- On supported third-party NFT marketplaces (Opensea, etc.) — the game recognizes ownership changes on-chain automatically

### Wallet Safety

- Player wallets are **read-write** for minting and trading.
- The game never requests full wallet permissions — only signing for specific actions.
- If a player's wallet is compromised, a **Recovery Grace Period** of 72 hours allows appeal to the Grand Counsel for asset escrow while a new wallet is linked.
## Card Collector's Guide

For players interested in the physical and digital collectible aspects of The Fifth Root, this guide covers how to build, preserve, and display a card collection.

### Collecting Basics

Every card in The Fifth Root has three properties relevant to collectors:

| Property | Description | Rarity Implication |
|----------|-------------|-------------------|
| **Card Number** | Position in the print run (e.g., "47 of 500") | Lower numbers are harder to obtain |
| **Print Date** | When the card was minted/printed | Earlier print dates predate balance patches |
| **Condition** | Physical card quality (Mint, Near-Mint, Played) | Affects resale value |

### Rarity Distribution

| Rarity | Approximate Print Run | Drop Rate from Sprouting/Rolls |
|--------|----------------------|-------------------------------|
| Common | 500–2,000 per set | ~65% |
| Uncommon | 200–800 per set | ~25% |
| Rare | 50–200 per set | ~8% |
| Legendary | 10–50 per set | ~2% |

### Preserving Physical Cards

Physical cards are printed on cardstock with a holographic finish on Legendary cards. To preserve condition:

- Store in sleeve protectors immediately upon receipt.
- Use top-loaders for long-term storage.
- Avoid direct sunlight — holographic finishes fade over time.
- Keep in a climate-controlled environment (extreme cold or heat can warp cardstock).

### Display and Trade

- **Guild Hall Display:** Legendary Character Cards and Trophy Cards can be displayed in the Guild Hall, visible to all guild members. This is purely cosmetic.
- **Character Card Portfolio:** Players can view their full card history (all tiers of Character Card, all Sprite cards earned) in the in-game Portfolio menu.
- **Community Card Shows:** The Grand Counsel may organize periodic in-game Card Show events where players can display their collections, trade, and earn cosmetic badges for rare completions.

### Card Set Rotation

The Fifth Root releases cards in sets tied to game milestones (e.g., "Season 1: The Root Awakening"). Each set has a distinct card back design. Older sets are not reprinted — once a print run is complete, those cards are permanently fixed in number.

Players who complete a full set (one of each card in a given set) receive the **Set Collector** title and a unique Legendary Character Card with a special holographic border.

> *"A card collected is a story kept."* — Root5 collector community saying

---

## Card Grading & Authentication

As the physical card market grows, The Fifth Root provides an integrated authentication and grading service to protect collectors and ensure the integrity of rare cards.

### The Aether Seal

Every physical card minted through the official Fifth Root pipeline includes an embedded **Aether Seal** — a holographic mark applied at print time that serves as the card's unique identity.

| Property | Description |
|----------|-------------|
| **Visual** | A thin holographic strip running vertically along the card's right edge, showing the Fifth Root root-symbol and card number when tilted |
| **Digital Link** | Each seal encodes a short verification hash that can be checked against the on-chain registry (see below) |
| **Tamper Evidence** | Attempting to remove or transfer the seal leaves visible damage to the cardstock. Seals cannot be reused |
| **Cost** | Included in the card's minting/printing fee — no additional charge for the Aether Seal |

### On-Chain Registry

All official physical cards have their Aether Seal hash and metadata stored in a public smart-contract registry on the Root5 supported network. Anyone can verify a card's authenticity by:

1. Reading the Aether Seal's verification hash (visible under magnification on the seal itself)
2. Querying the registry contract with that hash
3. Receiving the card's canonical metadata: card number, print run, rarity, mint date, and current ownership

This registry is **append-only** — once a card is printed and registered, its canonical data is locked. Ownership can be updated if the card is legitimately transferred or sold.

### Unofficial Grading

While The Fifth Root does not operate its own grading service (cards are sold as-is from the official pipeline), collectors may submit their cards to third-party grading services for professional condition assessment. The Aether Seal is designed to be compatible with standard graded-card holders — it is thin enough that the holographic strip remains visible through a slab's window.

The Grand Counsel periodically publishes a **Recommended Grader List** of third-party services that have demonstrated proper handling, storage, and transparency. Cards graded by a recommended grader receive a small cosmetic marker in the in-game Portfolio (a "Certified" badge) — this does not affect the card's on-chain metadata or gameplay utility.

### Lost or Damaged Cards

If a physical card is lost or damaged beyond usability:

- The on-chain digital twin **remains valid** — it can still be displayed in the in-game Portfolio and the card's digital art remains accessible.
- Physical reprints are **not available** for any card once its print run is complete (see Card Set Rotation above).
- If a card was stolen, the owner may declare it stolen in the registry, which marks it as **Flagged** in the public record. Flagging does not revoke the card's existence but may deter fraudulent resale.

### Counterfeit Protection

The Aether Seal's tamper-evident design and on-chain registry make large-scale counterfeiting impractical. For additional buyer protection:

- The official Fifth Root store is the only source of newly printed cards.
- Secondary-market buyers should verify the Aether Seal hash on-chain before purchase.
- Community-run Card Shows (see Card Collector's Guide) may require Aether Seal verification for high-value trades.

> *"A card without a seal is a leaf without a tree."* — Root5 printing master

---

## Sprite Trait Variant Cards

When a Sprite with a rare trait is evolved or reaches a Kinship milestone, its physical and digital card variants receive special authentication markers tied to that trait.

### Trait Authentication Seals

| Trait | Seal Appearance | In-Game Effect |
|-------|----------------|----------------|
| **Deep Echo** | Holographic strip shimmers with teal ripple effect | Card plays a soft resonance sound when scanned; digital card border pulses gently |
| **Sunforged** | Gold-foil overlay on the Aether Seal | Card glows faintly in direct light; digital card radiates particle sparkles |
| **Blightmarked** | Dark purple underlay beneath the Aether Seal | Card shows subtle shadow creep along edges; digital card has drifting mist animation |
| **Moonlit** | Silver micro-print along the seal edge | Card reflects ambient light differently; digital card border fades in/out like moon phases |
| **Thornweave** | Raised textured pattern on the seal surface | Card has tactile ridges; digital card sprouts small thorn animations on hover |

These trait seals are applied at card print time only — they cannot be added to existing cards retroactively. A trait-sealed card's authentication hash explicitly includes the trait metadata, so counterfeiters attempting to forge the visual effect will fail on-chain verification.

### Trading Premium

Sprite cards with trait seals trade for 15–40% above their base rarity value in the Guild Market, depending on trait scarcity:

- **Common traits** (Stubborn, Quickened, Deep-rooted) — no premium (too widespread)
- **Uncommon traits** (Windwhisper, Storm-touched, Moonlit, Thornweave) — +15% to +25%
- **Rare traits** (Deep Echo, Sunforged, Blightmarked) — +30% to +40%

The Grand Counsel publishes a quarterly **Trait Rarity Report** that updates these premiums based on current circulation numbers.

> *"Some seeds hum with echoes. Some burn with borrowed suns. The card remembers what the eye barely sees."* — Root5 collector codexHEREDOC
