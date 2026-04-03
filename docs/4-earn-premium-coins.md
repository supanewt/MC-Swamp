# How Players Earn Coins

Last updated: 2026-04-01
Server: `MC Swamp`

This file documents the current configured ways players can earn `Coins` on the server.

## Main Coin Sources

### 1. Rewards Menu

Players can claim timed rewards through `/rewards`.

- Hourly reward:
  - `+1` coin
- Daily reward:
  - `+5` coins
- Weekly reward:
  - `+25` coins

Source:

- `plugins/DeluxeMenus/gui_menus/rewards/rewards_menu.yml`

## 2. AFK Rewards

Players inside the `afk` region earn:

- `+2` coins every `15 minutes`

They also receive:

- `1x Common Key` every `60 minutes`

Source:

- `plugins/Skript/scripts/afk.sk`

## 3. Fishing Bonus

Fishing has a direct coin reward configured:

- `2%` chance on catch to receive `+2` coins

Fishing can also award crate keys, which can indirectly lead to more coins from crates.

Source:

- `plugins/Skript/scripts/customfishing.sk`

## 4. Level Rewards

Some level milestones grant coins directly when claimed through `/levels`.

Confirmed coin-paying levels:

- Level 1:
  - `+20` coins
- Level 4:
  - `+30` coins
- Level 7:
  - `+40` coins
- Level 10:
  - `+50` coins
- Level 13:
  - `+60` coins
- Level 15:
  - `+75` coins
- Level 18:
  - `+100` coins
- Level 21:
  - `+120` coins
- Level 23:
  - `+150` coins
- Level 24:
  - `+250` coins

Sources:

- `plugins/DeluxeMenus/gui_menus/levels/levels_1.yml`
- `plugins/DeluxeMenus/gui_menus/levels/levels_2.yml`

## 5. Crates

Crates can award Coins directly.

Confirmed crate payouts:

- Vote crate:
  - `25` or `50` coins
- Common crate:
  - `50` or `80` coins
- Rare crate:
  - `80` or `125` coins
- Epic crate:
  - `125` or `200` coins
- Superior crate:
  - `200` or `350` coins

Sources:

- `plugins/ExcellentCrates/crates/vote.yml`
- `plugins/ExcellentCrates/crates/common.yml`
- `plugins/ExcellentCrates/crates/rare.yml`
- `plugins/ExcellentCrates/crates/epic.yml`
- `plugins/ExcellentCrates/crates/superior.yml`

## 6. Envoys

CrazyEnvoys tiers include direct coin payouts.

Configured ranges found:

- Tier 1:
  - `20` to `40` coins
- Tier 2:
  - `40` to `70` coins
- Tier 3:
  - `50` to `100` coins
- Tier 4:
  - `75` to `150` coins
- Tier 5:
  - `250` to `500` coins

Sources:

- `plugins/CrazyEnvoys/tiers/Tier1.yml`
- `plugins/CrazyEnvoys/tiers/Tier2.yml`
- `plugins/CrazyEnvoys/tiers/Tier3.yml`
- `plugins/CrazyEnvoys/tiers/Tier4.yml`
- `plugins/CrazyEnvoys/tiers/Tier5.yml`

## Voting Note

Voting does **not** currently give direct Coins from the vote plugin itself.

Current vote rewards are:

- `1x Vote Key`
- `10 Level XP`

This means voting can still lead to Coins indirectly, because the `Vote` crate has coin rewards.

Source:

- `plugins/SuperbVote/config.yml`

## Currency Details

The server’s coin currency is managed by `CoinsEngine`.

- Currency name:
  - `Coins`
- Command aliases:
  - `/coins`
  - `/coin`
- Starting value for new players:
  - `0`

Source:

- `plugins/CoinsEngine/currencies/coins.yml`

## Short Summary

The main reliable ways to earn Coins are:

- claim `/rewards`
- AFK in the AFK zone
- fish for bonus rewards
- progress through `/levels`
- open crates
- win envoy drops

Indirect coin path:

- vote
  - voting gives Vote Keys
  - Vote Keys open Vote crates
  - Vote crates can pay Coins
