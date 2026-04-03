# How To Set Player Ranks

This server uses LuckPerms for rank management.

## Check Current Rank Info

```text
/lp user <player> info
/lp user <player> parent info
/lp groups
```

## Set A Permanent Rank

This replaces the player's current primary rank with the one you choose.

```text
/lp user <player> parent set <rank>
```

Examples:

```text
/lp user Steve parent set default
/lp user Steve parent set knight
/lp user Steve parent set lord
/lp user Steve parent set paladin
/lp user Steve parent set duke
/lp user Steve parent set king
/lp user Steve parent set youtuber
/lp user Steve parent set streamer
/lp user Steve parent set helper
/lp user Steve parent set builder
/lp user Steve parent set mod
/lp user Steve parent set srmod
/lp user Steve parent set admin
/lp user Steve parent set dev
/lp user Steve parent set manager
/lp user Steve parent set owner
```

## Add A Secondary Rank

This keeps their existing rank and adds another group.

```text
/lp user <player> parent add <rank>
```

Examples:

```text
/lp user Steve parent add youtuber
/lp user Steve parent add streamer
/lp user Steve parent add helper
```

## Remove A Rank

```text
/lp user <player> parent remove <rank>
```

Examples:

```text
/lp user Steve parent remove knight
/lp user Steve parent remove youtuber
/lp user Steve parent remove helper
```

## Set Donor Rank Track

Your donor progression ranks found in LuckPerms are:

```text
default -> knight -> lord -> paladin -> duke -> king
```

Use `settrack` so the player is placed correctly on that rank track.

```text
/lp user <player> parent settrack rank <rank>
```

Examples:

```text
/lp user Steve parent settrack rank default
/lp user Steve parent settrack rank knight
/lp user Steve parent settrack rank lord
/lp user Steve parent settrack rank paladin
/lp user Steve parent settrack rank duke
/lp user Steve parent settrack rank king
```

## Temporary Rank

```text
/lp user <player> parent addtemp <rank> <time>
```

Examples:

```text
/lp user Steve parent addtemp king 30d
/lp user Steve parent addtemp youtuber 7d
/lp user Steve parent addtemp helper 14d
```

## Promote Or Demote On The Donor Track

```text
/lp user <player> promote rank
/lp user <player> demote rank
```

Examples:

```text
/lp user Steve promote rank
/lp user Steve demote rank
```

## Rank Names On This Server

### Donor / Player Progression

```text
default
knight
lord
paladin
duke
king
```

### Media

```text
youtuber
streamer
```

### Staff

```text
helper
builder
mod
srmod
admin
dev
manager
owner
```

## Common Examples

Make a player `Knight`:

```text
/lp user Steve parent settrack rank knight
```

Make a player `King`:

```text
/lp user Steve parent settrack rank king
```

Give someone `Youtuber` in addition to their current rank:

```text
/lp user Steve parent add youtuber
```

Make someone `Mod`:

```text
/lp user Steve parent set mod
```

Remove a media rank:

```text
/lp user Steve parent remove streamer
```

## Notes

- Use `parent settrack rank` for the donor ladder so LuckPerms keeps the player on the proper progression track.
- Use `parent add` for extra groups like `youtuber`, `streamer`, or temporary staff-style access.
- `owner` may also rely on operator status outside of LuckPerms.
