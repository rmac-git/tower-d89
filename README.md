# Bastion Line

A browser tower defense game in one HTML file. There's no build step: open `index.html` in a browser.

## How to play

Hold the gate for 30 waves. If 20 lives' worth of enemies get through, you lose. After wave 30 you can keep playing in endless mode.

| Tower | Cost | Role |
|---|---|---|
| Archer (1) | 50g | Fast single-target shots, hits air |
| Mortar (2) | 90g | Splash damage, ground only |
| Frost Spire (3) | 70g | Pulses to slow everything in range |
| Tesla Coil (4) | 120g | Chain lightning, ignores armor |
| Longshot (5) | 150g | Long range and heavy hits; targets the strongest enemy by default |

Each tower has three levels. Selling refunds 70% of what you spent. Each tower can target **First**, **Last**, **Strong** or **Close**.

Enemies: Footman, Courier (fast), Ironclad (armored), Mite (swarms), Kite (flying, so Mortars can't hit it), Mender (heals nearby enemies), and a Warlord boss every 10 waves.

**Keys:** `1`–`5` pick a tower · `Space` sends the next wave (sending it early pays bonus gold) · `U` upgrades · `S` sells · `T` changes targeting · `F` changes speed · `P` pauses · `Esc` cancels.

## Tuning

All balance data is at the top of the script in `index.html`: `TOWERS`, `ENEMIES`, `SCRIPTED` waves, and the `hpMul` / `waveBonus` / `earlyBonus` curves. `window.__bastion` exposes the game state and core functions so you can run automated play-throughs.
