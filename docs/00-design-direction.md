# The Fifth Root — Design Direction (Canon v1.1)

**Status:** founder direction, 2026-10-18 (v1.1, 2026-10-17: Sap, ads, sign-in). This page overrides every other chapter where they disagree.
Chapters are being rewritten to match it, and until a chapter is updated, this page wins.
Every number marked *(tunable)* is a starting value. The game team sets the final value after playtests, and the DAO reviews prices each Season.

---

## 1. The game in one line

**Yu-Gi-Oh meets Zelda meets capture the flag.**

| Influence | What it means here |
|---|---|
| **Yu-Gi-Oh** (cards) | Every sprite you grow is captured into a **card**. You build a **deck** and **call your sprites out** of it to fight in training, quests and battles. |
| **Zelda** (adventure) | You explore regions, take on quests and dungeons, solve puzzles, beat bosses, and find seeds, items and keys. |
| **Capture the flag** (guild war) | Each of the four guilds has a **village with a flag**. Guilds defend their own village and raid the others. Village wins pay out to the players who fought. |

## 2. Three levels of play

Players rise through three tiers. Each tier opens a new layer of the world.

| Level | Tier | World layer | Unlocks |
|---|---|---|---|
| 1 | **Squire** | The **Guild Villages** and the lands around them: Training Arena, Greenhouse, shops, starter dungeons | Deck of up to 1 active sprite in battle, starter quests, village defense |
| 2 | **Warrior** | A **second region** beyond the villages, with harder quests, dungeons and bosses *(region name: proposal needed)* | 2 sprites per battle, counters, tier quests, raids on other villages |
| 3 | **Mage** | **The Aether level**: the realm of pure Aether around the Fifth Root | 3 sprites per battle, Aether abilities, final quests, Counsel seats |

To move up a tier you need the XP threshold **and** the tier's gate quest. You can't buy a tier.

## 3. A new player's first hour

1. **Create your character.** Lady (Rooth) or Lord (Root). **Choose your guild:** Ground, Fire, Water or Energy. Guilds are chosen, not rolled, so a player's Telegram guild team carries over.
2. **First training at the Training Arena, with Sap.** Sap, the oldest sprite, runs every village's Arena. This is the tutorial: move, fight, use an ability.
3. **Reward: your first Seed, from Sap's hands.** Every account gets exactly one free starter seed for finishing first training.
4. **Plant it at the Greenhouse**, where Seedagon the caretaker explains the growth options (§4).
5. **Start the first quest chain** while the seed grows.
6. **Sprout notification → mint → your first sprite card.** Now you can call it out in battle.

## 4. Sprite lifecycle (seed → sprout → card)

### 4.1 Getting seeds
| Source | Notes |
|---|---|
| Starter seed | 1 per account, for finishing first training |
| Greenhouse shop | Bought with ROOT5 *(tunable: 2,000 ROOT5)* |
| Quests and dungeons | Drop as loot |
| Other players | Bought in player shops or bartered |
| Lost in battle | A seed can be lost when running from a battle (§5.1) |

Seeds are **inventory items** (off-chain) until they sprout. Each seed has a **guild type** (Ground, Fire, Water, Energy), and the seed art already exists for all four.

### 4.2 Planting and growing
Plant the seed in a **Greenhouse garden plot**. The player then picks how it grows:

| Option | Cost | Time *(tunable)* | Effect on the sprite |
|---|---|---|---|
| **Watch an ad** | Free | Standard (3 days) | Normal start. Until ads are live, the "ad" is our own game trailer. |
| **Pay: Slow grow** | Low ROOT5 *(500)* | Long (5 days) | Must be **watered** a set number of times *(1 per day)*. Good care gives a **stronger** sprite. |
| **Pay: Fast grow** | High ROOT5 *(3,000)* | Short (12 hours) | No watering needed, but the sprite **starts weaker**. |
| **Hire the Caretaker** | ROOT5 fee per day *(150/day)* | Same as Slow | **Seedagon**, the Greenhouse caretaker, waters for you while you're out questing. Counts as full care. |

**Care Score (0–100).** Each watering, done on time, adds to the seed's Care Score, and missed waterings lower it. The Care Score sets the sprite's **starting strength**:

| Path | Starting stat multiplier *(tunable)* |
|---|---|
| Fast grow | ×0.85 |
| Ad grow, or Slow with poor care (score < 50) | ×1.00 |
| Slow with good care (50–89) | ×1.08 |
| Slow with perfect care (90–100) | ×1.15, and the species roll is made **twice, keep the one you prefer** (§4.5) |

The rule behind every option: **paying buys time, never power.** Fast costs more and gives a weaker sprite. The strongest sprites come from care.

### 4.3 Ready to sprout
When the seed is ready, the player gets a **notification** (in-game, plus Telegram, Discord or email, whichever they linked).

### 4.4 Minting the sprite
To sprout the sprite, the player either:
- **pays the mint fee** in ROOT5 *(tunable: 5,000)*, or
- **watches an ad** *(tunable: 1–3 views)*. The mint is then paid from the **Mint Faucet**, a pool funded by ad revenue and the game rewards reserve, with a daily cap per player and per game.

**On-chain format:** sprites are minted as **compressed NFTs (Metaplex Bubblegum v2) in a Metaplex Core collection.** A normal NFT costs about 0.003 SOL in account rent, which an ad view can't cover. A compressed NFT costs a tiny fraction of that, so the ad path is sustainable. *(Verify cost, trading support and attribute updates on devnet before launch.)*

### 4.5 Which sprite you get: the dice roll
At sprouting the game rolls **1d20**. The seed's guild type tilts the odds toward its own guild:

| Roll | Result |
|---|---|
| 1–10 | The sprite of the seed's guild (Ground → Seedagon, Fire → Onyx, Water → Fernad, Energy → Arbitos) |
| 11–13 | Next guild's sprite |
| 14–16 | The opposite guild's sprite |
| 17–19 | Previous guild's sprite |
| 20 | **The seed listens:** the player picks any of the four guild sprites |

- Guild order for "next / opposite / previous": **Ground → Fire → Water → Energy → Ground**.
- Every guild has the same odds. This fixes today's 1d12 table, where Ground was 4× more likely than Fire.
- **Perfect care** (Care Score 90–100) rolls twice and the player keeps the result they prefer.
- **The odds are published in the game.** Every result is a normal guild sprite, so a bought seed never hides a jackpot. Some countries regulate paid random rewards as loot boxes; equal-value results and published odds keep us on the safe side.
- **Sap is never in the roll.** Sap can't be grown from a seed (§4.7).
- **Traits** (rolled separately) add flavor. Care Score improves trait odds.

### 4.6 The sprite becomes a card
The sprouted sprite is **captured into a card** in the player's **card deck** (inventory). The card *is* the NFT: whoever holds the card owns the sprite. Cards can be:
- called out in training, quests and battles (§5)
- sold in player shops or bartered (§7)
- printed as a physical card with an NFC chip (§9)

Evolving a sprite **updates the same card** (stage, art and stats). There is no burn and re-mint, so the card's history and any NFC pairing stay intact.

### 4.7 Sap, the village elder (not a growable sprite)
Sap is the **oldest sprite**, made directly from Aether before any other creature (lore, chapter 01). He can't be hatched, bought or rolled.
- **Arena master of every village.** Lore: Sap's roots run under all four villages, and he rises in whichever Training Arena calls him. So every village has Sap, and he belongs to no guild.
- **He trains players and their sprites.** First training (the tutorial), sprite training sessions (sprite XP and Kinship, with a daily cap), sparring to practice before battles, and the **tier trials**: the Warrior and Mage gate quests end with a test in Sap's Arena.
- **He gives every new player their starter seed.**
- **He is a quest giver**, not a card anyone owns, so he stays the same for everyone and is never part of the economy.

**Proposal: Sap's Cutting** *(NEW: needs founder approval; if not approved, Sap stays a village elder only)*
- **What it is:** a way to earn a piece of Sap without ever capturing Sap himself.
- **How to earn it:** at the Aether level (Level 3), a Mage who wins **Sap's Trial** receives **Sap's Cutting**, a living sprig of Sap. The trial is a skill duel against Sap in the Arena, not a dice roll, and can be tried once per week.
- **What it does:** the Cutting is a **support card**. It can't attack. Its powers heal, restore SP and cleanse allies, and its strength is capped at the player's other sprites' level.
- **Limits:** one per player, ever. It's soulbound: it can't be sold, bartered or lost in battle. It's a trophy of mastery, so it never becomes a market jackpot.
- **Physical card:** it can be printed as a special NFC card.

## 5. Battles: deck, call-out, defend or run

- **Call out** a sprite card from your deck to fight. Squires can have 1 sprite out per battle, Warriors 2, Mages 3.
- When a sprite's HP hits 0 it is **wounded** and returns to the deck. Sprites never die; they heal over time or with healing items.
- With no sprites left standing, the player chooses:
  1. **Fight on alone** with their own weapons, abilities and items, or
  2. **Run.** Running always works, but costs **loot**.

### 5.1 What you can lose (run or defeat)
- The game takes **random items from your carried bag** *(tunable: 1–3 items, at most 10% of carried value)*.
- **Never a sprite.** Sprite cards (the NFTs) are never at risk.
- **Seeds can be lost**, because they are bag items.
- Items in your **village storehouse** are safe. Only what you carry is at risk, so packing for a quest is a real decision.
- **Against another player:** the lost items go to the winner.
- **Against an NPC or monster:** the lost items are **recirculated**, going back into loot tables and shop stock, not to anyone.

## 6. Guild villages and capture the flag

- Four villages (Ground, Fire, Water, Energy), each with a **flag**, a Training Arena, a Greenhouse, shops and a storehouse.
- **Defense is asynchronous.** Players register a **defender loadout** (character + sprite cards). Attackers fight those loadouts, controlled by the game's AI, at any time. Nobody has to be online at once.
- **Raids** run in scheduled windows (for example weekend evenings). Capturing a flag means beating a village's defender chain and reaching the flag.
- **Village wins pay out:** each Season week, villages score points from defenses, raids and flag captures. The ROOT5 village pool is shared among the winning village's players **in proportion to their contribution** *(capped per player)*.
- Flags captured are **trophies** (bragging rights and village decoration), not stolen assets.

## 7. ROOT5 in the game economy

### 7.1 Where ROOT5 goes in (spending)
| Spend | Examples |
|---|---|
| Skip time | Fast grow, Caretaker hire, instant heal, fast travel, quest timers |
| Greenhouse | Seeds, extra garden plots |
| Minting | Sprite mint (unless ad-paid) |
| Shops | NPC shop items, cosmetics, card frames, physical card printing |
| Market fees | 5% fee on player-shop sales |

### 7.2 Where ROOT5 comes out (earning)
| Earn | Rule |
|---|---|
| Quests and dungeons | Reward Points toward the weekly pool |
| Village wins | Share of the village pool by contribution |
| Referrals | Paid when the referred player **finishes first training and sprouts their first sprite**, not at sign-up. Both players earn. Capped per referrer per week. |
| Ads | Ad views pay for growth and mints through the faucet. They are not paid out as cash. |
| Community | Telegram activity XP converts to Reward Points (capped) |
| Selling | Sell cards, seeds and items to other players |

**All ROOT5 rewards come from a fixed weekly pool** (game rewards reserve, 15M ROOT5/year). Payouts can never exceed the pool, however many players or bots show up. There is no staking APY and no promised return.

### 7.3 Player shops and bartering
- **Player shops:** list items, seeds or cards for a ROOT5 price in your village stall or the marketplace (5% fee).
- **Bartering:** a direct item-for-item swap between two players, both confirm, no fee. ROOT5 can be added to either side.
- Fee split: part recycled into the rewards reserve, part burned, part to the DAO treasury (see Economy chapter).

## 8. Accounts without a crypto wallet

Many players won't want to manage a wallet. They don't have to:
Rule: **no paid wallet service and no private keys held by us.** Everything below uses free logins and the game's own account system.
- **Sign in with Telegram, Discord or email.** Telegram login is already how the Mini App works. Discord uses its free OAuth login. Email uses a one-time sign-in link. Each sign-in creates a **game account**, with no wallet needed.
- **A game account can do everything in the game:** grow seeds, hold cards, shop, barter, battle. Its ROOT5 balance and cards are kept in the **game ledger**, off-chain.
- **Cards stay "unminted" until a wallet is linked.** At sprout, the player still pays the mint fee or watches the ad. The card is fully playable at once. The NFT is minted to their wallet when they link one, paid from the Mint Faucet. Chain costs are only paid for players who want on-chain ownership.
- **Linking a wallet** (any time) is needed to **withdraw ROOT5** or **move cards on-chain**. Players who want a wallet without seed phrases can use Phantom's free Google or Apple login. Withdrawals have a cooldown *(tunable: 48 hours)* after linking a new wallet, and daily limits.
- **Trades between any accounts are ledger transfers.** A walletless player can buy from a wallet player, and the reverse. The seller's ROOT5 lands in their game balance and can be withdrawn by whoever has a linked wallet.
- **Backing:** the ledger's total ROOT5 is always covered by the game rewards wallet, which is checked daily and published.
- **Credits:** ad-faucet rewards and promo grants are **game credits**. They can be spent in the game but never withdrawn.
- Players with wallets (Phantom, Solflare, MetaMask for EVM holders) sign in by signing a message, as the web app already supports.
- Accounts can link several logins (Telegram + Discord + email + wallet), so a lost login doesn't lose the account.

## 9. Cards, physical cards and NFC

- **Digital card = the sprite NFT.** The deck is the player's set of cards.
- **Physical cards** can be ordered for minted cards. Each carries a **secure NFC chip** whose secret key can't be read or copied. Tapping the chip signs a fresh challenge, proving it's genuine. Details in `NFC_AUTH_SPEC.md`.
- Printed QR codes and printed hashes are **not** proof of authenticity, because they can be copied.

## 10. Ads (Bitmedia and placeholder)

- **Placeholder now:** the "ad" slot plays our own game trailer.
- **Bitmedia** (crypto-focused) supplies **banner ads** and **HTML5 / playable game ads** (a mini game inside the ad).
- **Banners:** menus, the Greenhouse, shops, the map, and the website. Never during a battle.
- **The "watch an ad" slot** (growth and mint): a **Sponsored Break** screen shows a Bitmedia HTML5 or playable ad for a fixed time *(tunable: 30 seconds)*. When Bitmedia has no ad to show, the game trailer plays instead.
- **Rewards are for the time on screen, never for clicks.** The reward unlocks when the server confirms the break ran its full time on a visible screen. One reward per break, daily caps per player, and bot checks.
- **Check with Bitmedia first** that a rewarded break is allowed under their publisher terms. Many ad networks ban rewarding users for viewing. If Bitmedia doesn't allow it, the reward slot uses our own trailer and direct sponsor videos, and Bitmedia stays on banners and non-rewarded playable ads.

## 11. Removed or changed from the current chapters

| Old rule (chapter) | Now |
|---|---|
| Ethereum and Polygon; player picks a chain at mint (06, 11, 13) | **Solana only** (compressed NFTs in a Core collection) |
| Staking with 4–15% APY (13) | **Removed.** No promised yields |
| Guild assigned by a 1d8 roll, plus a paid re-roll (02) | **Players choose** their guild |
| 1d12 sprout table, Ground-heavy (06) | **1d20 guild-weighted table** (§4.5), with published odds |
| Sap hatches on a 12; Sap scales infinitely with owner XP (06, 07, 11) | **Sap can't be hatched.** He's the Arena master and trainer in every village (§4.7). Sap's Cutting is a capped support card (proposal) |
| Embedded wallets from a paid vendor (v1 of this page) | **Free logins plus the game ledger**; mint and withdraw on wallet link (§8) |
| Seedagon farms 8 ROOT5/day; uncapped earnings (13) | Seedagon is the **Greenhouse caretaker** (paid). All earnings come from the capped weekly pool |
| Sprites "bound permanently" to a wallet (06) | Sprites are **tradeable cards** |
| Evolution burns and re-mints the NFT (06, 11) | Evolution **updates the same card** |
| Raids take 50% of the loser's sprites (09) | **Sprites are never lost.** Only bag items are, and only on running or defeat |
| Flee is a 1d6 roll with no stakes (07) | **Run always works**, but costs random bag items (§5.1) |
| "Historical data shows…" (13) | **Never state invented figures as history** |

## 12. Rules for anyone writing the docs (people or agents)

1. This page is canon. If a chapter disagrees, fix the chapter, not this page.
2. Don't add a **new system** without a written proposal. Extending an existing system is fine.
3. Put tunable numbers in a **Parameters** table at the end of each chapter, not scattered through the text.
4. Use real time ("3 days"), not "in-game days".
5. Never present invented statistics as facts or history.
6. Keep in-game governance (Counsel, Root Keeper) separate from the real DAO treasury. In-game votes never move real funds.
