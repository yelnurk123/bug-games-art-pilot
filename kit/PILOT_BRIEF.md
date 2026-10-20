# Art direction pilot · stage 1: style sheet and three pilots

You are the chat that made this game, so you know how its look is made. bug.games needs your game's art for its platform: posters, small marks, stills, store and pass art. Before any of that is made, we agree on the look. This stage is small: one sheet and three pieces.

**Dry run.** Don't write to the game's workspace, don't publish, and don't declare any products or pass for review.

## Read
0. **`VISUAL_LANGUAGE.md` with `reference/` open.** What bug.games looks like, the For You wall your poster joins, and every place your art goes. Look at every picture before you start.
1. `GRAMMAR.md`: how bug.games judges art (10 minutes).
2. `EXAMPLES.md` and `examples/`: four posters that work, and why. Don't copy them.
3. `STYLE_SHEET.template.md`: what to fill in.

## Make
1. **`STYLE_SHEET.md`**, from the template, written from the game itself.
   - Use 4–6 reference frames from the game's own key art, cover or renderer, saved as files beside the sheet.
   - Measure every ink with `python3 tools/measure.py colour '#hex' …` (always with the `#`).
   - Measure the 2:1 poster with `python3 tools/measure.py light poster.png`.
2. **Three pilots**, finished, in the game's ORIGINAL art style:
   - **`pilot-poster.png`**: 1600×800 (2:1), the For You poster.
     - One image, your register, two to four inks.
     - No title lettering, and nothing essential in the bottom 26 px.
     - Must read at 90×70.
     - The wall crops it into 13 shapes, from a 3.5:1 strip to a 1:2 column, around one focus point. Name your focus point in the style sheet.
     - Take the medium, line, inks and characters from your key art; leave its lettering, buttons and crowd behind (VISUAL_LANGUAGE.md §3).
   - **`pilot-icon.png`**: 92×92, drawn for display at 46 px. Your last survivors only; not the poster shrunk.
   - **`pilot-store-item.png`**: 400×400.
     - One look a player could own (a skin, a companion, a trim), shown on your world's own ground.
     - It changes looks, never the game's identity core.
     - No price on it.
3. **Run `python3 tools/wall.py pilot-poster.png --title "<Game>" --focus x,y --icon pilot-icon.png`** and hand in the `wall-hero.png` and `wall-shapes.png` it writes.
4. **`PREVIEW.png`**: one sheet showing the three pilots beside 2–3 of your reference frames, plus the poster at 90×70 and the icon at 46 px on a black ground and on a linen (#F1ECE4) ground.
5. **`QUESTIONS.md`**: anything you can't decide from the game itself. Never invent a price or a rule.

## What makes a pilot fail
- It doesn't look like the game: a plain engine screenshot, a different line or a different texture.
- It doesn't read at 90×70 (poster) or 46 px (icon), or its one image is lost in the wall's shapes.
- It's the key art squeezed: title lockup, buttons, the whole cast, or a busy background.
- Numbers, prices or title lettering on the poster.
- A colour within 12 ΔE of ember, lilac or sun used as a flat block, or where Play, a price or a selected state will sit.
- The game's own colours changed to pass a check (keep the real hex; follow its zone's rule).
- A picture whose light doesn't come from the source it shows (one source, and the light visibly comes from it).

## Hand in
1. Work on a branch named **`pilot-v1`**.
2. Put everything in **`handin/v1/`**: STYLE_SHEET.md, the reference frames, the three pilots, wall-hero.png, wall-shapes.png, PREVIEW.png and QUESTIONS.md.
3. Push the branch and open a pull request titled **"<Game> · art pilot v1"**.

bug.games replies on that pull request, and in **`reply/v1/`** on the same branch: your pilots on the real wall, and "approved" or specific notes. The next version goes in `handin/v2/` on a branch named `pilot-v2`. Never merge the pull request yourself.

Only after approval comes stage 2: a sketch sheet of every slot, which is also the plan for anything the game doesn't have yet (a store, a pass, achievements).
