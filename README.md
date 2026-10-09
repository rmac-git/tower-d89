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

**Field orders:** from wave 10 on, before every fifth wave you pick one of three perks. Each gives a bonus and a cost, such as +20% damage for +1 enemy armor.

**Enemies:** Footman, Courier (fast), Ironclad (armored), Mite (swarms), Kite (flies straight to the gate along the dotted line, so Mortars can't hit it), Mender (heals nearby enemies), and a Warlord boss every 10 waves.

**Maps:** Switchback (long and winding), The Serpent (four long climbs), Short Fuse (a short road, hard). Your best wave is saved per map.

**Keys:** `H` commands the hero · `E` / `R` hero skill and ultimate · `K` skill tree · `1`–`5` pick a tower · `Space` sends the next wave (sending it early pays bonus gold) · `U` / `I` pick upgrade path A / B · `S` sells · `T` changes targeting · `Q` / `W` abilities · `N` next-wave intel · `Esc` closes menus · `F` changes speed · `P` pauses · `M` mutes · `Esc` cancels.

## Learning curve

The game starts simple and adds one system at a time. Each unlock arrives with a short message on the board, and new towers get a NEW badge.

| After clearing wave | Unlocks |
|---|---|
| Start | Archer, Mortar, your hero |
| 1 | Hero signature skill |
| 2 | Frost Spire |
| 3 | Barrage |
| 4 | Tesla Coil |
| 5 | Longshot |
| 6 | Level 3 upgrade paths |
| 7 | Cold Snap |
| 8 | Tower targeting |
| 9 | Field orders (then every fifth wave) |
| 20 | Hero ultimate |

The skill tree button (★) appears with the hero's first skill point. The first wave shows tips on the board.

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

The game is built for landscape and the battlefield always takes as much of the screen as possible. On wide-short screens such as phones in landscape, the stats and build menu sit in a narrow rail on the left and the controls, hero and abilities in a rail on the right. On other screens they sit in slim strips above and below the board. Tap a tower in the build rail to expand its stats like an accordion (tap again to collapse). Tower and wave details appear in a small floating card only while something is selected, and on phones a placed tower's card has a Show stats toggle (the ⓘ button or `N` shows next-wave intel). In portrait on a touch device the game shows a "Turn your phone sideways" screen (with a "Play in portrait anyway" button) and pauses until you rotate. Tapping **Take command** also requests full screen and a landscape lock where the browser allows it.

On touch screens, drag a tower from the build menu onto the map; the preview floats just above your finger and turns red where you can't build. Tapping a tower and then tapping a tile twice (preview, then confirm) also works. Tapping near a built tower selects it.

**Feedback:** blocked actions explain themselves on the board ("Can't build on the road", "Need 40 more BST", "Barrage ready in 8s"). A green arrow floats over any tower you can afford to upgrade. The box next to Send wave previews the next wave's enemies (hover or long-press for names). Losing a life flashes the board.

**Settings (⚙):** sound, full screen, larger text, and quit to title (tap twice to confirm).

## Tuning

All balance data is at the top of the script in `index.html`: `TOWERS` (including each `br` path), `ENEMIES`, `MAPS`, `PERKS`, `ABIL`, `SCRIPTED` waves, and the `hpMul` / `waveBonus` / `earlyBonus` curves. `window.__bastion` exposes the game state and core functions so you can run automated play-throughs.
