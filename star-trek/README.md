# Star Trek (fan tribute)

A from-scratch homage to the classic text-mode **Star Trek** game: the 1971 mainframe
original, the 1978 *Super Star Trek* rewrite, and the many DOS versions that followed.
It runs in an 80x25 text-mode screen with 16 CGA/EGA colors, a ship's log, a DOS-style
function-key bar and PC-speaker-style sound.

It's one self-contained file with no dependencies. **Open `index.html` in any modern browser to play.**
(It loads the VT323 terminal font from Google Fonts when online and falls back to a
system monospace font offline.)

## Your mission

Klingon battle cruisers have invaded the galaxy. Hunt down and destroy all of them
before the stardate deadline. The galaxy is an 8x8 grid of **quadrants**, and each
quadrant is an 8x8 grid of **sectors**. Starbases can refuel, rearm and repair you,
but only when you dock next to one.

## Commands

Type the first three letters of a command, press its function key, or click the bar.
You can put the numbers on the same line, like `NAV 3 1` or `PHA 500`.

| Command | Key | What it does |
| --- | --- | --- |
| `NAV` | F2 | Set a course (1-9) and warp factor (warp 1 = one quadrant) |
| `SRS` | | Short range scan report (the scanner is always on screen) |
| `LRS` | F9 | Long range scan of the neighboring quadrants |
| `PHA` | F3 | Fire phasers (spends energy, split across every Klingon here) |
| `TOR` | F4 | Fire a photon torpedo on a course |
| `SHE` | F5 | Move energy into or out of the shields |
| `DAM` | F6 | Damage report, plus repairs when docked |
| `COM` | F7 | Library computer: chart, status, torpedo data, starbase nav, calculator, region names |
| `CHA` | F8 | Galactic chart (click a quadrant to fly there) |
| `HELP` | F1 | Command list and the course compass |
| `XXX` | | Resign your command |
| | F10 | Sound on/off |

Courses go counter-clockwise, and fractions like `2.5` are allowed:

```
  4  3  2
   \ | /
 5 --<*>-- 1
   / | \
  6  7  8
```

**Point and click:** click a Klingon on the short range scanner to fire a torpedo at it,
click empty space or a starbase to fly there, and click a quadrant on the long range scan
or galactic chart to warp to it. The game types out the matching command so you can
learn the syntax. Up and Down recall earlier commands, and Esc cancels a prompt.

## Tips

- **Raise your shields before a fight.** Klingon hits come off your shields, and if
  they drop below zero the Enterprise is destroyed.
- Klingons shoot back after every phaser shot, every torpedo and every move.
- Phaser damage falls off with distance. Torpedoes kill in one hit, but stars block them.
- Damaged systems slowly repair as you travel. At a starbase you can repair everything
  at once (`DAM`).
- Each jump between quadrants takes a full stardate, whatever the warp factor.

## What's in it

- The 1978 *Super Star Trek* rules: 8 ship systems that can be damaged, the Klingons'
  shooting and repositioning, the Starfleet dialogue and the Antares-to-Spica region names.
- Three ranks: Ensign, Captain (the classic game) and Admiral.
- An efficiency rating when you win, with your best rating per rank saved in your browser.
- Scanner effects for phaser beams, torpedo tracks, explosions and warp jumps.

This is an unofficial fan project and isn't affiliated with CBS Studios or Paramount.
