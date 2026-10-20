# Style sheet · <GAME TITLE>

Your game's look, described in the bug.games grammar (GRAMMAR.md). Every asset you make later is judged against THIS sheet, not against anyone's taste. Write it from the game itself: its key art, its renderer, its cover. Keep it to one page plus the frames.

## 1. In one breath
- **Three words** for how the game feels:
- **One sentence** on the world:
- **The one image** (the single shape or object that holds the game, readable at 90×70):
- **Focus point** of the 2:1 poster (x, y as fractions; the wall crops around it, see `tools/wall.py`):
- **Register** (silhouette / stage / edition) and why:

## 2. Reference frames (4–6)
Frames from the game's own key art, cover or renderer, not new drawings. For each: what it shows, and what it proves about the look (line, light, texture, lettering, a character).

| # | File | What it shows | What it proves |
|---|---|---|---|

## 3. Rules of the look
Write each as a rule someone else could check.
- **Line:** how edges are made (or not made).
- **Fill:** flat, shaded, textured, hatched, built from parts…
- **Texture:** what surfaces are made of; what never appears.
- **Lighting:** where light comes from; what is bright, what is dark.
- **Composition:** how a picture is built (subject, floor, sky, framing); how the bottom 26 px stays quiet.
- **Lettering:** the title's own letterforms; where lettering may appear; its minimum size.
- **Characters and voice:** how beings are drawn; how they emote; the one verb of the game.
- **Motion gait** (if anything moves): stepping, snap, slow…; the reward moment in 3 frames (start, peak, held).

## 4. Small marks
- **Last survivors** (2–3 things that must remain at 46 and 30 px):
- How the marks are made at small size (drawn on a grid, hand-placed, simplified…):

## 5. Palette, measured
Run `python3 tools/measure.py colour '#hex' …` (with the `#`) on every ink.

| Ink | Hex | Role | ember / lilac / sun ΔE | Zone (free / caution / guarded) | How a guarded ink is used |
|---|---|---|---|---|---|

- **Light band of the 2:1 poster:** run `python3 tools/measure.py light poster.png` and record L, C and the band.

## 6. Never
What this game's art never does: list the style's own "nevers" first, then the platform's. The platform's: no numbers in stills, no lettering on shrinkable plates, guarded colours never as button-like fills or near Play, prices or selected states, no other game's art.

## 7. Questions
Anything you can't decide from the game itself. Never guess a price or a rule.
