# MC Swamp Tebex Package Checklist

Use this as the package entry list for `store.mcswamp.com`.

## Setup Order

Create Tebex categories in this order:

1. Coins
2. Ranks
3. Crate Keys
4. Utility
5. Cosmetics
6. Claimblocks
7. Backpacks
8. Furniture

## Coins

These should be your first live products.

### 100 Coins

- Category: `Coins`
- Price: choose your real USD price
- Commands:

```text
coins give {username} 100
```

### 250 Coins

- Category: `Coins`
- Price: choose your real USD price
- Commands:

```text
coins give {username} 250
```

### 500 Coins

- Category: `Coins`
- Price: choose your real USD price
- Commands:

```text
coins give {username} 500
```

### 1000 Coins

- Category: `Coins`
- Price: choose your real USD price
- Commands:

```text
coins give {username} 1000
```

### 2500 Coins

- Category: `Coins`
- Price: choose your real USD price
- Commands:

```text
coins give {username} 2500
```

### 5000 Coins

- Category: `Coins`
- Price: choose your real USD price
- Commands:

```text
coins give {username} 5000
```

### 10000 Coins

- Category: `Coins`
- Price: choose your real USD price
- Commands:

```text
coins give {username} 10000
```

## Ranks

### Knight Rank

- Category: `Ranks`
- In-game value: `2000 Coins`
- Commands:

```text
lp user {username} parent settrack rank knight
```

### Lord Rank

- Category: `Ranks`
- In-game value: `4000 Coins`
- Commands:

```text
lp user {username} parent settrack rank lord
```

### Paladin Rank

- Category: `Ranks`
- In-game value: `6000 Coins`
- Commands:

```text
lp user {username} parent settrack rank paladin
```

### Duke Rank

- Category: `Ranks`
- In-game value: `8000 Coins`
- Commands:

```text
lp user {username} parent settrack rank duke
```

### King Rank

- Category: `Ranks`
- In-game value: `10000 Coins`
- Commands:

```text
lp user {username} parent settrack rank king
```

## Crate Keys

### 1x Common Key

- Category: `Crate Keys`
- In-game value: `50 Coins`
- Commands:

```text
crate key give {username} common 1
```

### 5x Common Keys

- Category: `Crate Keys`
- Commands:

```text
crate key give {username} common 5
```

### 1x Rare Key

- Category: `Crate Keys`
- In-game value: `100 Coins`
- Commands:

```text
crate key give {username} rare 1
```

### 5x Rare Keys

- Category: `Crate Keys`
- Commands:

```text
crate key give {username} rare 5
```

### 1x Epic Key

- Category: `Crate Keys`
- In-game value: `150 Coins`
- Commands:

```text
crate key give {username} epic 1
```

### 5x Epic Keys

- Category: `Crate Keys`
- Commands:

```text
crate key give {username} epic 5
```

### 1x Superior Key

- Category: `Crate Keys`
- In-game value: `250 Coins`
- Commands:

```text
crate key give {username} superior 1
```

### 5x Superior Keys

- Category: `Crate Keys`
- Commands:

```text
crate key give {username} superior 5
```

## Utility

### /Back

- Category: `Utility`
- In-game value: `200 Coins`
- Commands:

```text
lp user {username} permission set essentials.back true
```

### /Feed

- Category: `Utility`
- In-game value: `300 Coins`
- Commands:

```text
lp user {username} permission set essentials.feed true
```

### /Heal

- Category: `Utility`
- In-game value: `500 Coins`
- Commands:

```text
lp user {username} permission set essentials.heal true
```

### /Repair

- Category: `Utility`
- In-game value: `750 Coins`
- Commands:

```text
lp user {username} permission set essentials.repair true
```

### /Fly

- Category: `Utility`
- In-game value: `1500 Coins`
- Commands:

```text
lp user {username} permission set essentials.fly true
```

## Claimblocks

### 100 Claimblocks

- Category: `Claimblocks`
- In-game value: `2 Coins`
- Commands:

```text
adjustbonusclaimblocks {username} 100
```

### 1000 Claimblocks

- Category: `Claimblocks`
- In-game value: `20 Coins`
- Commands:

```text
adjustbonusclaimblocks {username} 1000
```

### 10000 Claimblocks

- Category: `Claimblocks`
- In-game value: `200 Coins`
- Commands:

```text
adjustbonusclaimblocks {username} 10000
```

## Backpacks

### Leather Backpack

- Category: `Backpacks`
- Unlock: `9 slots`
- In-game value: `25 Coins`
- Commands:

```text
lp user {username} permission set backpack.use true
lp user {username} permission set backpack.size.1 true
```

### Bronze Backpack

- Category: `Backpacks`
- Unlock: `18 slots`
- In-game value: `50 Coins`
- Commands:

```text
lp user {username} permission set backpack.use true
lp user {username} permission set backpack.size.1 true
lp user {username} permission set backpack.size.2 true
```

### Silver Backpack

- Category: `Backpacks`
- Unlock: `27 slots`
- In-game value: `100 Coins`
- Commands:

```text
lp user {username} permission set backpack.use true
lp user {username} permission set backpack.size.1 true
lp user {username} permission set backpack.size.2 true
lp user {username} permission set backpack.size.3 true
```

### Higher Backpack Tiers

- Category: `Backpacks`
- Source file:
  - `/home/supanewt/workspace/plugins/DeluxeMenus/gui_menus/coinshop/coinshop_backpacks.yml`
- Notes:
  - Keep higher tiers cumulative.
  - Include all lower backpack permissions in the Tebex package.

## Cosmetics

These are strong store products because they are low-risk for balance.

### Hats

Suggested starter packages:

- Astronaut Hat
- Cool Hat
- Diamond Hat
- Batman Hat

Example commands:

```text
lp user {username} permission set ultracosmetics.hats.Astronaut true
lp user {username} permission set ultracosmetics.hats.Cool true
lp user {username} permission set ultracosmetics.hats.Diamond true
lp user {username} permission set ultracosmetics.hats.Batman true
```

### Pets

Suggested starter packages:

- Piggy Pet
- Dog Pet
- Frog Pet
- Axolotl Pet

Example commands:

```text
lp user {username} permission set ultracosmetics.pets.piggy true
lp user {username} permission set ultracosmetics.pets.dog true
lp user {username} permission set ultracosmetics.pets.frog true
lp user {username} permission set ultracosmetics.pets.axolotl true
```

### Particle Effects

Suggested starter packages:

- Snow Cloud
- Angel Wings
- Inferno
- Ender Aura

Example commands:

```text
lp user {username} permission set ultracosmetics.particleeffects.snowcloud true
lp user {username} permission set ultracosmetics.particleeffects.angelwings true
lp user {username} permission set ultracosmetics.particleeffects.inferno true
lp user {username} permission set ultracosmetics.particleeffects.enderaura true
```

### Projectile Effects

Suggested starter packages:

- Rainbow
- Flame
- Love
- Portal

Example commands:

```text
lp user {username} permission set ultracosmetics.projectileeffects.Rainbow true
lp user {username} permission set ultracosmetics.projectileeffects.Flame true
lp user {username} permission set ultracosmetics.projectileeffects.Love true
lp user {username} permission set ultracosmetics.projectileeffects.Portal true
```

### Death Effects

Suggested starter packages:

- Explosion
- Firework
- Lightning

Example commands:

```text
lp user {username} permission set ultracosmetics.deatheffects.Explosion true
lp user {username} permission set ultracosmetics.deatheffects.firework true
lp user {username} permission set ultracosmetics.deatheffects.Lightning true
```

## Furniture

Suggested starter furniture packages:

- Bed
- Piano
- Sofa
- Fireplace

Commands:

```text
furniture give bed {username}
furniture give piano {username}
furniture give sofa {username}
furniture give fireplace {username}
```

## Toolskins

### Random Toolskin Voucher

- Category: `Cosmetics` or `Toolskins`
- In-game value: `25 Coins`
- Commands:

```text
crazyvouchers:voucher give Random_Toolskin 1 {username}
```

## Best First Launch List

If you want the smallest clean launch, start with only these:

1. 100 Coins
2. 250 Coins
3. 500 Coins
4. 1000 Coins
5. 2500 Coins
6. Knight Rank
7. Lord Rank
8. Paladin Rank
9. 1x Common Key
10. 1x Rare Key
11. 1x Epic Key
12. 1x Superior Key
13. /Fly
14. /Repair
15. 1000 Claimblocks

## Good Pricing Method

To price Tebex packages cleanly:

1. Pick a base cash value for `100 Coins`.
2. Scale all other packages from that.
3. Keep Tebex prices slightly better than manual one-by-one value.

Example pricing model:

- 100 Coins = `$1.99`
- 250 Coins = `$3.99`
- 500 Coins = `$6.99`
- 1000 Coins = `$11.99`
- 2500 Coins = `$24.99`

You can then price direct products according to their Coin cost.

## Notes

- Best launch approach: sell Coins first, then let players use `/coinshop`.
- Safest direct Tebex products: ranks, keys, cosmetics, utility perks.
- Avoid leading with direct cash or direct top-tier gear.

