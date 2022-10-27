## Kirby: Battle Royale - Gateway codes

**[РУССКИЙ](https://github.com/Injector/WitcherDeveloperConsole/blob/main/README.md)**

V 1.0
Last updated 27.10.2022

Screenshots: https://imgur.com/a/AulYupd

Works only on game version **3.0 EUR**!

My first experience in creation gateway codes, all of these tested in Citra Nightly build 1797 and Citra android.
These codes should work on Nintendo 3Ds.
Gateway codes are created via Cheat Engine Debugger (find out what writes to this address) and built in Android version Memory viewer by weihuoya

I started this project to play as Axe Knight in singleplayer and battle royale.

## Notes

About play as codes, they are changes your ability and other players in the battle, not in the menu.
Singleplayer codes works in the multiplayer, but **Client-Side**, means other players **won't* see your new ability (maybe one day I'll create multiplayer codes)
Also they can desync multiplayer actions. So don't use them in the multiplayer.

If you do not have the desired ability, restart the battle 1-3 times, until it appears. If it still doesn't, restart the game.

Avoid usage both play as codes in singleplayer and play as codes in training. Use one of them, because of possibly code conflicts and game breaks.

Where ``YYYYYYYY``, paste an ID from the list, check out them in Ability ID List and Color ID List

## Play as (Singleplayer, Not Cake Royale)

This code changes your ability in the battle to selected id. You can use it to play as unplayable characters (B. W. Dee, Waddle Dee Soldier, Axe Knight)

```
D3000000 30000000
2062E298 YYYYYYYY
2062E2B4 YYYYYYYY
2062EEA4 YYYYYYYY
2062E2AC YYYYYYYY
D2000000 00000000
```

# Play as (Cake Royale Story mode)

```
D3000000 30000000
216E78C4 YYYYYYYY
D2000000 00000000
```

# Player 2 play as (Singleplayer)

```
D3000000 30000000
2062E334 YYYYYYYY
D2000000 00000000
```

# Player 3 play as (Singleplayer)

```
D3000000 30000000
2056E6D0 YYYYYYYY
2062E3D0 YYYYYYYY
D2000000 00000000
```

# Player 4 play as (Singleplayer)

```
D3000000 30000000
2062E46C YYYYYYYY
D2000000 00000000
```

# Play as in Training Mode (Singleplayer, from menu)

```
D3000000 30000000
22204C50 YYYYYYYY
D2000000 00000000
```

# Set color (Singleplayer)

Use color ID from Color ID List

```
D3000000 30000000
2062E5EC YYYYYYYY
D2000000 00000000
```

## Play as (Singleplayer, alt code)

```
D3000000 30000000
216E7880 YYYYYYYY
216E7920 YYYYYYYY
216E791C YYYYYYYY
D2000000 00000000
```

## Ability ID list

| Ability | ID | Name | Based on |
| ------ | ------ | ------ | ----- |
| Sword | ``00000000`` | Sword | |
| Bomb | ``00000001`` | Bomb | |
| Tornado | ``00000002`` | Tornado  | |
| Ninja | ``00000003`` | Ninja | |
| Beetle | ``00000004`` | Beetle | |
| Parasol | ``00000005`` | Parasol | |
| Hammer | ``00000006`` | Hammer | |
| Cutter | ``00000007`` | Cutter | |
| Doctor | ``00000008`` | Doctor | |
| Spear | ``00000009`` | Spear | |
| Ice | ``0000000A`` | Ice | |
| Fighter | ``0000000B`` | Fighter | |
| Whip | ``0000000C`` | Whip | |
| WaddledeeParasol | ``0000000D`` | Waddlee Dee Parasol | |
| Metaknight | ``0000000E`` | Meta Knight | |
| Dedede | ``0000000F`` | King Dedede | |
| Mirror | ``00000010`` | Mirror | |
| Sleep | ``00000011`` | Sleep | |
| WaddledeeBuddy | ``00000012`` | Bandana Waddlee Dee | Waddlee Dee Parasol |
| WaddledeeSpear | ``00000013`` | Soldier Waddlee Dee | Spear |
| AxeKnight | ``00000014`` | Axe Knight | Cutter |

You can check these abilities in ``mint/Default.bin.cmp`` class ``Scn.Game.Hero.AbilityKind``

## Color ID list

| Color | ID |
| ------ | ------ |
| Pink | ``00000000`` |
| Yellow | ``00000001`` |
| Green | ``00000002`` |
| Blue | ``00000003`` |
| Gray | ``00000004`` |
| Orange | ``00000005`` |

You can check these colors in ``mint/Default.bin.cmp`` class ``Scn.Game.Hero.ColorKind``
