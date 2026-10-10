# Hold the Cove

A browser tower defense game in one HTML file. There's no build step: open `index.html` in a browser.

## How to play

The game is a campaign across three maps, ten waves each: Switchback (waves 1–10), The Serpent (11–20) and Short Fuse (21–30). When a map is held you march to the next one: towers stay behind but are salvaged for their full cost, lives refill to 20, and your hero, skills, story, upgrade unlocks and field orders carry over. A checkpoint is saved at the start of every map, so the title screen offers **Continue**. The title screen is kept to the name, one line and the buttons, and each map is introduced when you reach it. and losing lets you **Retry this map** instead of starting over. After wave 30 you can keep playing in endless mode.

| Tower | Cost | Role | Level 3 paths |
|---|---|---|---|
| Archer (1) | 50g | Fast single shots, hits air | Ranger (rapid fire) or Ballista (ignores armor) |
| Mortar (2) | 90g | Splash damage, ground only | Bombard (huge blast) or Napalm (burning) |
| Frost Spire (3) | 70g | Pulses to slow enemies | Glacier (periodic freeze) or Blizzard (damage) |
| Tesla Coil (4) | 120g | Chain lightning, ignores armor | Storm (10 jumps) or Arc Lance (one huge bolt) |
| Longshot (5) | 150g | Long range, heavy hits | Assassin (armor-piercing) or Gunner (fast fire) |

**Build sites:** towers go on stone build sites beside the road, 12 per map (11 on Short Fuse), not on any open tile. Sites are placed so each one covers road the others don't, and no two touch. While you're placing a tower the open sites glow, and a click or tap anywhere near a site snaps to it. Towers are drawn about a third larger than before and hit 1.55× harder, so a few well-developed towers do the work that used to take dozens. Most of your BST goes into upgrading, choosing paths and mastering the towers you have. Saved games with towers on old non-site tiles get those towers refunded at full cost.

The second upgrade splits into two paths, so two players end up with different defenses. Selling refunds 70% of what you spent. Each tower can target **First**, **Last**, **Strong** or **Close**.

**Veterancy:** towers earn rank from their own fighting. A kill is worth 1 point, and an assist is worth ½. An assist is an enemy the tower hurt that something else finished off, so Frost Spires and other support towers rank up too. The ranks are Recruit, Seasoned (25), Veteran (75), Elite (180) and Legend (400). Each rank adds 6% damage and 3% fire rate. A promotion flashes gold over the tower and announces the new rank. Gold stars on the tower's stone base show its rank, and the tower panel shows its kills, assists and how far it is to the next rank. Veterancy is kept in saves. It doesn't carry to a new map, because towers are salvaged when you march on.

**Compare before you buy:** select a tower and hover an upgrade, path or mastery button (or tab to it) to preview it. The stats list shows each value as current ▲ new or current ▼ new, so better and worse don't depend on colour. Every stat any of the options touches is listed, so the panel doesn't jump while you compare. On the map the tower shows its upgraded form, and a dotted blue ring shows the new range. On touch screens the first tap previews and a second tap on the same button buys; tapping the other option switches the comparison.

**Mastery (after wave 8):** once a tower is in its final form, it can learn one of two skills and rank that skill up three times. Choosing one skill locks the other for that tower, so two Archers can end up very different. Rank costs are 1.2×, 2× and 3× the tower's build cost. Small diamonds under the tower show its rank: orange for the first skill and blue for the second. `U` and `I` pick a skill, then `U` buys the next rank. Undo works on mastery too.

| Tower | Skill A | Skill B |
| --- | --- | --- |
| Archer | **Volley**: also fires at 1/2/3 more enemies for half damage | **Eagle Eye**: 20/30/40% chance to crit for 3× damage |
| Mortar | **Shrapnel**: +20/40/60% blast radius, +10/20/30% damage | **Concussion**: stuns the blast for 0.3/0.45/0.6s (once every 2s per enemy, shorter on Warlords) |
| Frost Spire | **Deep Freeze**: stronger, longer slow and more range | **Shatter**: chilled enemies take +15/30/45% damage from everything |
| Tesla Coil | **Overload**: +2/4/6 chain jumps, +10/20/30% damage | **Static**: every enemy hit is slowed 25/35/45% |
| Longshot | **Headhunter**: +10/20/30% damage, plus +60/120/180% more to Ironclads and Warlords | **Ricochet**: bounces to 1/2/3 more enemies at 40% damage |

**Abilities:** your hero's two skills are the only special abilities (see Heroes). The old Barrage and Cold Snap buttons were retired so there are fewer buttons and each one matters more.

**Field orders:** from wave 10 on, before every fifth wave you pick one of three perks. Each gives a bonus and a cost, such as +20% damage for +1 enemy armor.

**Enemies:** Footman, Courier (fast), Ironclad (armored), Mite (swarms), Kite (flies straight to the gate along the dotted line, so Mortars can't hit it), Mender (heals nearby enemies), and a Warlord boss every 10 waves.

**Maps:** Switchback (long and winding), The Serpent (four long climbs), Short Fuse (a short road, hard), played in that order. Your best wave is saved.

**Keys:** `B` opens the build gallery · `H` commands the hero · `E` (or `Q`) aims the hero's signature skill, then click the map · `R` (or `W`) ultimate · `K` hero skills card · `1`–`5` pick a tower · `Space` sends the next wave (sending it early pays bonus gold) · `U` / `I` pick upgrade path A / B · `S` sells · `T` changes targeting · `Q` / `W` abilities · `N` next-wave intel · `Z` or `Ctrl`/`Cmd`+`Z` undoes your last build, upgrade or sale · `Esc` closes menus · `F` changes speed · `P` pauses · `M` mutes · `Esc` cancels.

## Learning curve

The game starts simple and adds one system at a time. Each unlock arrives with a short message on the board, and new towers get a NEW badge.

| After clearing wave | Unlocks |
|---|---|
| Start | Archer, Mortar, your hero |
| 1 | Hero signature skill |
| 2 | Frost Spire |
| 4 | Tesla Coil |
| 5 | Longshot |
| 6 | Level 3 upgrade paths |
| 8 | Tower targeting |
| 8 | Tower mastery |
| 9 | Field orders (then every fifth wave) |
| 20 | Hero ultimate |

The hero's ultimate unlocks at hero level 5 (usually near the end of the first map). The first wave shows tips on the board.

## Heroes

After picking a map you choose a hero who fights on the field beside your towers. Click or tap the hero (or press `H`) to command them, then click anywhere to send them there. Heroes gain experience from nearby kills, level up to 10, and fall and respawn if overrun.

Following Bloons TD 6's pattern (a light ability early, a big one later, both improving automatically) and avoiding the skill-tree busywork reviewers criticised in Kingdom Rush 5, each hero has exactly **two special skills**:

- **Signature skill (`E`):** available from wave 1. It's aimed: press it, then click or tap anywhere on the map. It ranks up on its own at hero levels 3 and 7, and each rank adds something you can see.
- **Ultimate (`R`):** unlocks at hero level 5 and ranks up at level 9.

| Hero | Signature (E) | Rank 2 (lv 3) | Rank 3 (lv 7) | Ultimate (R, lv 5) | Ultimate rank 2 (lv 9) |
|---|---|---|---|---|---|
| Maren Voss, Warden of the Gate | **Leap Slam**: leaps to the spot and slams it (damage and stun) | Knocks enemies back down the road | An aftershock slams again | **Hold the Line**: 8s unkillable fury, nearby towers +30% fire rate | The banner stuns everything near her every 2.5s |
| Ilse Kaur, the Ember Scribe | **Meteor**: a burning meteor on the spot | Leaves burning ground for 4s | Two smaller meteors chase it in | **Sunfall**: twelve meteors | Twenty meteors, each leaving burning ground |
| Tick Brannock, the Gate Tinker | **Sentry Drop**: an auto-turret that fires for 12s | Sentry overclocks nearby towers (+50% fire rate) | Two sentries | **Total Overclock**: every tower 2× fire rate, +50% damage for 8s | Lasts 12s and recharges Sentry Drop |

Big moments shake the screen a little (off with **Fewer effects**). Heroes also grow passively with every level: Maren toughens, regenerates and later cleaves; Ilse hits harder and later sets enemies alight; Tick reaches further and boosts towers near him. The ★ button (or `K`) opens a card showing both skills, what each rank adds, and at which level.

**Story:** each hero has a prologue and five chapters (after waves 5, 10, 15, 20 and 25) following the fall of the High Marshal, Corvane. Chapter 2 asks you to choose how the hero's signature skill evolves (for example, Meteor becomes Cataclysm or Meteor Shower, and Sentry Drop becomes Overdrive or Arc Reactor). The victory epilogue changes with your choice.

## The BST token

All prices and rewards use **BST**, the game's in-game token (the hex coin with a castle on it). BST is off-chain: there is no wallet, no blockchain and no real value. It exists only in the current game session and resets each run.

## Phones and tablets

The game is built for landscape and the battlefield always takes as much of the screen as possible. On wide-short screens such as phones in landscape, the stats and build menu sit in a narrow rail on the left and the controls, hero and abilities in a rail on the right. On other screens they sit in slim strips above and below the board. Tap a tower in the build rail to expand its stats like an accordion (tap again to collapse). Tower and wave details appear in a small floating card only while something is selected, and on phones a placed tower's card has a Show stats toggle (the ⓘ button or `N` shows next-wave intel). In portrait on a touch device the game shows a "Turn your phone sideways" screen (with a "Play in portrait anyway" button) and pauses until you rotate. Tapping **Take command** also requests full screen and a landscape lock where the browser allows it.

**Build gallery:** the Build button (or `B`) opens a gallery of every tower with its art, cost, stats and level 3 paths. The battle pauses while it is open, and stays paused while you place the tower you picked, then picks up where it was. Esc or right-click cancels. Keys `1`–`5` still pick a tower directly on desktop. On touch screens, tap a stone site to preview the tower and tap it again to place it. Tapping near a built tower selects it.

**Layout:** the battlefield takes most of the screen. Your BST balance sits at the top of the control rail in large type, with lives and map progress beneath it. On wide screens such as phones in landscape the rail runs down the right side; otherwise it is a single strip across the top.

**Feedback:** blocked actions explain themselves on the board ("Can't build on the road", "Need 40 more BST", "Meteor ready in 8s"). A green arrow floats over any tower you can afford to upgrade. The box next to Send wave previews the next wave's enemies (hover or long-press for names). Losing a life flashes the board.

**Settings (⚙):** sound, full screen, larger text, and quit to title (tap twice to confirm).

## Settings

The gear menu has **Sound** (a quick mute, also `M`), **Full screen** on phones, **Settings** and **Quit to title**. The title screen has a Settings link too. Settings are kept on this device. The panel pauses the game while it's open and has:

- **Sound:** separate Music and Sound effects volumes.
- **Gameplay:** **Send waves automatically** starts the next wave 3 seconds after one is cleared (it stops at the end of each map). **Pause when you leave** pauses the game and silences it when you switch apps or tabs.
- **Display and accessibility:** **Larger text**. **Bigger shots** makes arrows, shells, bolts and lightning about 1.7× larger, like the projectile-size option in Bloons TD 6. **Fewer effects** cuts sparks and flashes, and turns on automatically if your device asks for reduced motion. **Vibration** buzzes when you lose a life, a Warlord arrives or the gate falls; it only appears on devices that support it, which excludes iPhones.
- **Progress:** **Reset progress** erases saves and your best wave, after a second tap to confirm.

## Music

**If you can't hear anything:** sound starts on your first tap, and any later tap or key press wakes it up again after you switch apps. On iPhone and iPad the game asks for the media audio channel, so it plays even with the ring/silent switch on silent. The device's media volume still applies, and so does the Sound toggle in the ⚙ menu (`M`). A reminder appears when you start a game with sound turned off.

The soundtrack is an original piece written for the game, in a Maritime indie tropical house style: 4/4 at 108 BPM in G major, with a 16-bar loop (an 8-bar "low tide" hook and an 8-bar "high tide" lift over G–D–Em–C). It is played live by Web Audio with no audio files.

- **Between waves:** squeezebox (accordion-style) pads, offbeat marimba in a 3-3-2 pattern, and a penny-whistle hook with a dotted-eighth echo. The hook rests every other A section so it doesn't wear out.
- **During a wave:** a soft four-on-the-floor kick, claps on 2 and 4, a shaker and a sub bass join in, and the pads duck under each kick (sidechain pumping).
- **When a Warlord appears:** the pad filter opens up and the hats double to sixteenths.

## Saving

The game saves itself. After every wave, and whenever you build, upgrade or sell between waves, it records your towers, BST, lives, hero, skills and field orders. Close the page at any point and **Continue** on the title screen picks up at the next wave. Quitting in the middle of a wave takes you back to the start of that wave. A choice you were in the middle of, such as field orders or the map-held screen, is offered again.

Saves live in the browser. When the game is opened as an artifact on claude.ai, it also keeps a private copy in your account (the artifact's `db` storage, under your own user, so nobody else can read it). That copy follows you to other devices, and whichever save is newer wins. If you lose a map, the autosave is dropped and **Retry this map** or **Continue** restarts that map from its first wave.

## Mistakes

Undo takes back your last build, upgrade or sale with a full refund. The Undo button next to Build (or `Z`, or `Ctrl`/`Cmd`+`Z`) works for 10 seconds of game time. Its tooltip shows how many seconds are left, and the button hides once there is nothing left to undo. Undoing several times in a row steps back through your recent actions.

Double-clicks are absorbed. A second click or tap within 0.4 seconds of picking a tower, building, upgrading or selling is ignored. Double-clicking a gallery card won't also drop a tower on the map, double-clicking Upgrade buys only one level, and double-tapping a tile on a phone only previews it. Holding down `U`, `I`, `S` or `Z` doesn't repeat the order.

## Colour-blind friendly

The palette is safe for protanopia and deuteranopia. Good and bad are shown as sky blue and orange, never green and red. Invalid build spots get an orange outline and an X. Every enemy has its own shape as well as a colour from the Okabe-Ito palette:

| Enemy | Shape | Colour |
| --- | --- | --- |
| Footman | Circle | Yellow |
| Courier | Dart | Sky blue |
| Ironclad | Square | Pale grey |
| Mite | Small dot | Pink |
| Kite | Flapping diamond | White |
| Mender | Hexagon with a plus | Blue |
| Warlord | Star with a crown | Orange |

All enemies have dark outlines, and the same shapes appear in the next-wave peek and the scouting report. Health bars go from blue to yellow to orange.

## Art direction

Low-poly and flat-shaded, lit from the top-left. The map is a jittered triangle mesh shaded from a gentle height field: a green Nova Scotia meadow, a warm sand road with a darker bank, and soft build pads on every open tile. The Atlantic runs along the bottom. Its pink-granite shoreline rises and falls, and one or two rounded coves cut into the meadow. The shore is lined with lupins and a red-and-white lighthouse. A geodesic glamping dome takes a 2×2 block near the middle, with a cedar deck, string lights and a fire pit. Three 2×2 fenced pastures off the road hold wandering chickens, goats and rabbits, and there are spruce stands and granite boulders. There is also a cave mouth where enemies emerge, and a stone keep at the gate. Towers stand on faceted stone plinths and grow taller and add parts as they level (studs on the plinth count levels, and a coloured gem marks the chosen path). Following Kingdom Rush's approach, each upgrade changes the silhouette, not just the stats. Heroes are drawn a quarter larger than before. Each turns to face what it's attacking, steps and bobs while walking, and breathes while idle. Each also has its own moving details. **Maren Voss** is an armoured knight with a T-visored helm, a waving red plume, a swaying cape, a kite shield painted with a lighthouse, and a banner on her back that grows and glows during Hold the Line. **Ilse Kaur** wears a starry robe, a scarf that streams behind her and a crooked witch's hat. Her ember staff glows, and a spellbook floats beside her with glowing pages. **Tick Brannock** is a goggled tinker with a steam-puffing backpack, a spinning gear, a blinking antenna, a scoped rifle, a tool belt, and a little scout drone that circles overhead. A dashed ring in the hero's colour turns slowly under their feet, and a glow surrounds them while their ultimate is active.

## Tuning

The board is a 16 × 10 grid of 60px tiles (`TILE`, `COLS`, `ROWS`), with `SPEED_K` and `RANGE_K` tuning enemy speed and tower reach for that grid. All balance data is at the top of the script in `index.html`: `TOWERS` (including each `br` path), `ENEMIES`, `MAPS`, `PERKS`, `ABIL`, `SCRIPTED` waves, and the `hpMul` / `waveBonus` / `earlyBonus` curves. `window.__bastion` exposes the game state and core functions so you can run automated play-throughs.
