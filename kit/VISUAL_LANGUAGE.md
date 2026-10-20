# What bug.games looks like, and how your game shines in it

Read this with the pictures in `reference/` open. They are bug.games' own design boards: the Home page, a game page, events, the session result, the share card and the profile. They show the frame your art will live in. The posters and characters in them belong to other games on the platform. Look at them to understand the frame, never to copy, trace or borrow them.

Some parts of the boards are marked PROPOSAL or PROPOSED. Treat those parts as direction, not final specs.

## 1. The page is quiet so the games can be loud

- The page is near-black ink, with sharp corners and thin seams. Titles use a plain grotesque. Labels are small, spaced mono capitals. The chrome has no gradients, no glows and no rounded cards.
- On Home, the posters are the only colour. Your poster isn't competing with the interface. It's competing with the twelve other posters next to it.
- Four colours carry meaning, and only the platform uses them for that:
  - ember: Play, Continue, Join;
  - lilac: selected, yours;
  - sun: crumbs and rewards;
  - mint: owned.

  That's why your art never uses them as flat fills near those controls (see GRAMMAR.md).

## 2. Why the wall works (`01-home-for-you-wall.png`)

Look at the For You wall. Every poster is made in a different medium:

- a paper print with an offset double (Carbon Body)
- a whale made of dots in a lighthouse beam (Night Swim)
- a pixel portrait (Mind Your Brother)
- a tile pattern under a sun (Miradouro)
- comic rays (Inkstrike)
- a typewriter page (Typos)
- an embroidery hoop (Seam Ripper)
- a wireframe spider (Threadbare)

Even so, the posters belong together, because each one:

- **is one idea you can say in five words.** "A whale of stars in a beam", not "the cast and the world".
- **is built from big flat shapes in two to four inks.** It reads across a room and at 90 px.
- **has attitude.** A wink, a stamp, a glare, a bomb with a grin: wit, not decoration.
- **carries no title, logo, button, number, HUD or tagline.** Typos is the one exception: an Edition poster, where the lettering is the art.
- **fills its slot edge to edge, on its own ground.** It has no frame, no border and no vignette.

**A poster shines here by being the most "itself" thing on the wall, not the most detailed.**

## 3. Your key art is not your poster

Your game's key art, cover and title screen were made for pages the game controls. They usually carry:

- a title lockup;
- a "play" button;
- the whole cast lined up;
- bursts, taglines and badges.

On bug.games the platform prints the title, the button and every number. So:

- **Take from your key art:** the medium, the line, the inks, the light, the characters and their attitude.
- **Leave behind:** the lettering, the buttons, the crowd and the busy background.
- **Choose:** one character in one moment, or one object in one light. The rest of your world appears when the poster moves, and when the game page opens.

## 4. The wall reshapes your poster

The wall has 13 slots, and they aren't all 2:1. These are the picture areas measured on the board in `01`, in px:

| Shape | Size | Ratio |
|---|---|---|
| No 1 (hero) | 685×319 | 2.1 : 1 |
| Strip | 577×163 | 3.5 : 1 |
| Wide | 443×149 | 3 : 1 |
| Band | 288×126 | 2.3 : 1 |
| Tall | 236×316 | 3 : 4 |
| Half | 288×316 | about 1 : 1 |
| Column | 140×305 | 1 : 2 |
| Small | 237×137, 200×137 | |
| Tile | 137×126 | |

- The platform crops your 2:1 poster around one **focus point**. Put your one image near it, and surround it with a ground that can be cut away.
- A **24 px caption strip** on night sits under every poster. It holds your title and number, printed by the platform. Keep the bottom 26 px of the art free of anything essential.
- **Status chips** (NEW, LIVE, STAFF PICK, NO 1 THIS WEEK) sit on the bottom-left corner of the picture. Keep that corner calm.
- **Check it yourself:** `python3 tools/wall.py pilot-poster.png --title "Your Game" --focus 0.5,0.5 --icon pilot-icon.png`. It writes:
  - `wall-hero.png`: your poster in the No 1 slot of the real wall;
  - `wall-shapes.png`: your poster in every shape.

  If your one image is lost in the tall shapes at every focus, say so in QUESTIONS.md and show a 2:3 cut beside it. `examples/` has 2:3 versions of the four example posters.

## 5. Every other place your art goes

| Picture | What it shows | What your game supplies there |
|---|---|---|
| `02-home-featured-and-live` | the Featured banner; the Live & next cards | the banner art (the platform puts its copy beside it); event art under a status chip |
| `03-home-vibes-and-lists` | the vibe tiles and the game lists | in list rows, only a small thumbnail: your icon or the centre of your poster |
| `04-game-page-hero` | your game's page | your world is the backdrop; the platform's info card, tags and Play sit on the right |
| `05-game-page-event-and-store` | Live this week and the store | the event plate; each store item on your world's own ground; the price row is the platform's |
| `06-game-page-creator-and-more` | Made by, Shape it, More like this | the creator's art; your poster again, reused |
| `07-game-page-phone` | the whole page on a phone | the same art, stacked; check that it still reads |
| `08`–`12` event pictures | an event on Home, compact and in the inbox, the studio entry, and a second event | event banner art with the left part kept plain for the copy |
| `13-continue-your-place` | Continue on Home | one still of your game as a window, plus a small marker (read the notes on the image) |
| `14-session-result` | the end of a session | the moment your game rewards; the numbers are the platform's |
| `15-share-card` | the share card on phones | the picture; your title lettering is allowed here |
| `16-profile` | a player's profile | your poster as a favourite; your small marks and seals in Played lately |

## 6. Before you hand in, ask

1. Look at `wall-hero.png` from across the room. Is yours the most "itself" poster on the wall? Can you name its one image in five words?
2. Could anyone mistake it for one of its neighbours?
3. In `wall-shapes.png`, does the one image survive every shape and 90×70?
4. Does your icon still say your game at 46 px, on night and on linen?
5. Is anything on it the platform's job: a title, a button, a number, a price?
