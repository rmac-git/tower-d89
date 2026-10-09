# Bastion Line

A browser tower defense game in one HTML file. There's no build step: open `index.html` in a browser.

## How to play

Hold the gate for 30 waves on one of three maps. If 20 lives' worth of enemies get through, you lose. After wave 30 you can keep playing in endless mode.

| Tower | Cost | Role | Level 3 paths |
|---|---|---|---|
| Archer (1) | 50g | Fast single shots, hits air | Ranger (rapid fire) or Ballista (ignores armor) |
| Mortar (2) | 90g | Splash damage, ground only | Bombard (huge blast) or Napalm (burning) |
| Frost Spire (3) | 70g | Pulses to slow enemies | Glacier (periodic freeze) or Blizzard (damage) |
| Tesla Coil (4) | 120g | Chain lightning, ignores armor | Storm (10 jumps) or Arc Lance (one huge bolt) |
| Longshot (5) | 150g | Long range, heavy hits | Assassin (armor-piercing) or Gunner (fast fire) |

The second upgrade splits into two paths, so two players end up with different defenses. Selling refunds 70% of what you spent. Each tower can target **First**, **Last**, **Strong** or **Close**.

**Abilities:** *Barrage* (`Q`, 40s cooldown) drops five armor-piercing shells on a patch of road you choose. *Cold Snap* (`W`, 55s) slows every enemy for five seconds.

**Field orders:** before every fifth wave you pick one of three perks. Each gives a bonus and a cost, such as +20% damage for +1 enemy armor.

**Enemies:** Footman, Courier (fast), Ironclad (armored), Mite (swarms), Kite (flies straight to the gate along the dotted line, so Mortars can't hit it), Mender (heals nearby enemies), and a Warlord boss every 10 waves.

**Maps:** Switchback (long and winding), The Serpent (four long climbs), Short Fuse (a short road, hard). Your best wave is saved per map.

**Keys:** `H` commands the hero · `E` / `R` hero skill and ultimate · `K` skill tree · `1`–`5` pick a tower · `Space` sends the next wave (sending it early pays bonus gold) · `U` / `I` pick upgrade path A / B · `S` sells · `T` changes targeting · `Q` / `W` abilities · `F` changes speed · `P` pauses · `M` mutes · `Esc` cancels.

## Heroes

After picking a map you choose a hero who fights on the field beside your towers. Click or tap the hero (or press `H`) to command them, then click anywhere to send them there. Heroes gain experience from nearby kills, level up to 10, and fall and respawn if overrun.

| Hero | Style | Skill (E) | Ultimate (R, after wave 20) | Skill paths |
|---|---|---|---|---|
| Maren Voss, Warden of the Gate | Melee, charges nearby packs | Shockwave: damage and stun around her | Last Stand: can't fall, hits harder, nearby towers speed up | Bulwark · Vanguard · Banner |
| Ilse Kaur, the Ember Scribe | Ranged mage, ignores armor | Meteor on the densest pack | Sunfall: twelve meteors | Cinder · Aether · Lantern |
| Tick Brannock, the Gate Tinker | Ranged engineer | Overclock nearby towers | Total Overclock: every tower, double speed | Rifle · Workshop · Scavenger |

**Skill tree (`K`):** three paths of three tiers per hero. Tiers cost 1, 2 and 3 points, and each needs the one above it. Points come from levels and from story chapters 2 and 4, so you can't learn everything in one run.

**Story:** each hero has a prologue and five chapters (after waves 5, 10, 15, 20 and 25) following the fall of the High Marshal, Corvane. Chapter 2 asks you to choose how the hero's skill evolves (for example, Meteor becomes Cataclysm or Meteor Shower). Chapter 4 unlocks the ultimate. The victory epilogue changes with your choice.

## The BST token

All prices and rewards use **BST**, the game's in-game token (the hex coin with a castle on it). BST is off-chain: there is no wallet, no blockchain and no real value. It exists only in the current game session and resets each run.

## Phones and tablets

The game is built for landscape. In portrait on a touch device it shows a "Turn your phone sideways" screen (with a "Play in portrait anyway" button) and pauses until you rotate. On a phone in landscape the board fills the screen height, the build menu and abilities sit to its right, and nothing scrolls the page. Tap **Take command** to also request full screen and a landscape lock where the browser allows it (a Full screen button appears on touch devices).

Touch building is two taps so small tiles are easy to hit: pick a tower, tap a grass tile to preview it, then tap the same tile again to build. Tapping near a built tower selects it.

## Tuning

All balance data is at the top of the script in `index.html`: `TOWERS` (including each `br` path), `ENEMIES`, `MAPS`, `PERKS`, `ABIL`, `SCRIPTED` waves, and the `hpMul` / `waveBonus` / `earlyBonus` curves. `window.__bastion` exposes the game state and core functions so you can run automated play-throughs.
