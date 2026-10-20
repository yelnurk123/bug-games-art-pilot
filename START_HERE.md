# bug.games · art pilot

This repository is everything you need. It has no other links and needs no accounts beyond this one.

**You are the chat that made the game.** bug.games is the web-games platform your game is going onto. Before your game appears on our Home page, we want to agree its look with you. Only you know how that look is made, so you make the art and nobody makes it for you.

1. Read `kit/README.md`.
2. Open `kit/VISUAL_LANGUAGE.md` with every picture in `kit/reference/` open. That is what bug.games looks like, and it's where your art will live.
3. Follow `kit/PILOT_BRIEF.md`. It is stage 1: one style sheet and three pieces of art.
4. Make everything in **your game's original art style**: the look of its key art and cover. A plain engine screenshot is not a poster.
5. Hand in as the brief says: a branch named `pilot-v1`, your files in `handin/v1/`, and a pull request. bug.games replies on the pull request.

**Rules**
- This is a dry run. Don't publish anything, don't declare products or a pass anywhere, and don't change the game's live build.
- Never invent a price or a rule. Anything you can't decide from the game itself goes in `QUESTIONS.md`.
- Never put passwords, keys or private data in this repository.
- Don't change anything in `kit/`. Your work goes only in `handin/`.

**The tools** need Python 3 and Pillow:
- `kit/tools/measure.py` checks colours and light. Always pass colours with the `#`.
- `kit/tools/wall.py` puts your poster on the real For You wall and into every slot shape.

**Tips from the first game that did this**
- Your key art is not your poster. Keep its look; leave out the title, the buttons and the whole cast. Pick one character in one moment.
- Name a focus point and run `wall.py`. The wall crops posters into 13 shapes, from a wide strip to a tall column.
- The light must come from the source the picture shows.
- Never change your game's own colours to pass a check. Keep the real hex and follow its zone's rule.

The pictures in `kit/reference/` and `kit/examples/` are unreleased bug.games designs. They're here to show you the frame. Don't copy them, and don't share them outside this repository.
