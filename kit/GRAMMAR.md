# The bug.games poster grammar

How art for bug.games is judged. It applies to every game, whatever its style. Read it to understand what the platform needs. Then describe your own game's look in these terms, in your style sheet. You don't change your style; you translate it.

## The one idea underneath

**The frame makes the games a collection, not a shared style.** No two games on bug.games look alike, and none should. What they share is the platform's frame: thin ink seams between posters, one caption strip under each, one stamp style, one Play colour. bug.games frames and curates. It never repaints a world in house style, and a game never invents its own frame, border or caption.

**So:** your art stays exactly yours. The platform gives every game the same frame. Your job is to make your world read inside that frame, at every size it will be shown.

## The principles

1. **Find the one image.** Before drawing anything, name the single silhouette or object that holds the game: a figure, a lit window, a creature, an object. If it doesn't read at 90×70 pixels, it isn't the image.
2. **Keep your game's own medium.** Pixel stays on its pixel grid, paper stays paper, clay stays clay, dots stay dots. Make every piece the way your game makes its world. A plain screenshot is not a poster: a poster is composed, lit and finished for its slot, in the game's style.
3. **Choose a register for the wall.** Every poster is one of three:
   - **Silhouette:** one shape holds the world. It survives every squeeze.
   - **Stage:** one lit pocket in the dark.
   - **Edition:** printed lettering is part of the art. This is rare: one loud poster and one quiet sheet per wall.

   Pick the one that suits your game. Say it in your style sheet.
4. **Two to four inks, one of them your game's own.** Fewer inks read better at small sizes.
5. **Detail lives where the eye lands.** There's one clear path for the eye at rest. The rich world is revealed by motion and when the poster is opened, not crammed into the still.
6. **The still is the poster.** Design the held frame first: it's what people see with reduced motion, in a share and in an email. Motion adds; it never rescues a weak still.
7. **Lettering belongs to the caption.** The platform prints your title in the strip under the poster. Put title lettering on the art only on pieces that never shrink below about 200 px wide, such as the share card and event art, and only with letters at least 12–18 px tall.
8. **The bottom 26 px is the caption strip.** Nothing essential goes there.
9. **Small marks are drawn, never shrunk.** Icons are shown square with sharp corners, never masked to a circle. At 64 px and below, the poster is replaced by marks drawn for that size: icon 46, emblem 30, and optionally chip 64. Name your **last survivors**, the two or three things that must remain at the smallest size (for example, a hood and two eyes).
10. **No numbers in pictures.** Posters, stills and reward tiles carry no counts, prices or scores. The platform prints every number. A HUD inside a running gameplay loop is allowed, because it's part of the game.

## Platform colours stay the platform's

The platform uses four colours for meaning:

- **ember** #FF5A36 = act (Play, Join, Buy)
- **lilac** #C4B5FF = selected / yours
- **sun** #FFCB57 = money and rewards
- **mint** #7FE3C0 = owned

A game never recolours these, and the platform never recolours a game. If one of your colours is close to them, it gets a rule, not a change:

| Distance to a platform colour (ΔE2000) | Zone | Rule |
|---|---|---|
| under 12 | **Guarded** | Allowed in the art, but never as a button-like flat fill (a block or pill 24×24 px or bigger, or one carrying text or a number). Never within 120 px of the matching control: Play for ember, a price for sun, a selected state for lilac |
| 12–20 | **Caution** | Only the 120 px rule applies |
| 20 or more | **Free** | No rule |

Measure with `tools/measure.py colour '#rrggbb' …`. Always include the `#`. It also reports mint; whether the 120 px rule applies near the owned check isn't decided yet, so just report it.

**Never recolour your own game to pass a zone.** A close colour gets a rule, not a change: keep the game's real hex and follow the rule for its zone.

## On the wall: light and loudness

The For You wall alternates light and dark posters, and rations loudness. Measure your 2:1 poster with `tools/measure.py light poster.png`. It gives L (lightness) and C (colourfulness):

| Band | Threshold |
|---|---|
| Dark | L under .20 |
| Mid | L .20 to .50 |
| Light | L .50 or more |
| Loud | C .45 or more |
| Quiet sheet | L .85 or more and C .08 or less |

On the wall:
- no two light posters touch;
- no two loud posters touch;
- two mid posters touch only if their L differs by .10 or more.

Dark next to dark is tolerated. You don't choose your slot; the platform places games by these rules. Report your band so the platform can place you.

## Motion (when your poster moves)

- One living thing per region. Only a few posters move at once; the rest show their still.
- **Never animate** prices, dates, counts, type, Play or captions.
- Reveals come through a surface (a wipe, a push, a cut on action), never a cross-fade.
- **The world sets the gait:** stepping for pixel and stop-motion worlds, snap-then-overshoot for loud ones, slow for quiet ones.

## Who owns what

| | The platform owns | Your game owns |
|---|---|---|
| For You wall | seams, caption strip, stamps, Play, slot | the poster (still and motion), its register, palette, medium |
| Game page | chrome, tabs, Play, prices, every number | backdrop, what sections sit on, the reward moment |
| Store | price row, buy, "Yours" (all under the art, in the platform's chrome, never over it) | item art on your own ground; looks only, never your identity core |
| Pass | rail, step count, state marks | pass name, step unit, reward art, row grounds |
| Seals | name, rule, rarity, "earned" | the seal: an outline by kind (feat / collection / event) plus one glyph, states drawn in your world; never gold, never a padlock |
| Event | copy zone, dates, counter, Join | banner art with the left ~45% kept plain for copy |
| Share card | a linen bug.games bar | the picture; your title lettering is allowed here |

## The test for any asset

1. Is it unmistakably your game, in your game's own style?
2. Does it read at the size it will be shown?
3. Does it leave the platform's job (numbers, buttons, captions, colours of meaning) to the platform?
4. Could it be mistaken for another game? If yes, it's wrong.
