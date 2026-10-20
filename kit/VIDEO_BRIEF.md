# Gameplay video: an optional brief

A gameplay video is **optional**. If your game doesn't want one, that's fine: your gallery pictures and your poster carry the page.

If you make one, it is **not a cinematic trailer**. It is **real play from your current build, the best bits cut together**, and it opens on your most powerful moment. The same video goes on your game page and on social media.

## Why it's made this way
People decide in a second or two, usually with the sound off. A video that starts with a logo or a slow build-up loses them. One that starts in the middle of your best moment, with the game visibly being played, keeps them.

## The shape

| Beat | Time | What it shows |
|---|---|---|
| **Hook** | 0–2 s | Your most powerful real moment: the peak of your core verb, a near miss, the big reaction. **The very first frame is already gameplay.** |
| **What you do** | 2–8 s | The core loop, clearly: your one verb, twice |
| **It gets better** | 8–25 s | 3–6 short beats (1.5–4 s each), one feature each: a second mechanic, a new place, a character, playing together. Each one a step up |
| **Peak** | last 3–5 s | Your best payoff, without spoiling what you keep secret |
| **End** | ~1.5 s | bug.games' end card: your title lockup and "Play free on bug.games". You supply the lockup; we add the card |

## Make three cuts from the same takes

| Cut | Format | Length | For |
|---|---|---|---|
| **Page** | 16:9, 1920×1080 (at least 1280×720), 30 or 60 fps | 20–45 s | Your game page gallery |
| **Vertical** | 9:16, 1080×1920, re-framed (no black bars) | 15–30 s | TikTok, Reels, Shorts, phone shares |
| **Micro** | the first 6 s of the page cut | 6 s | Home cards, link previews |

- **Files:** MP4 (H.264 video, AAC audio at 48 kHz), in the highest quality you have.
- **Page cut:** keep the action inside the **central 4:3** of the frame (1440×1080), because phones show a narrower crop.
- **Vertical cut:** keep action and text out of the apps' buttons: roughly **220 px at the top, 450 px at the bottom and 150 px on the right**. Check on a phone.
- **Sound:** it must make sense **muted**. Use your game's own sound, and music only if you own it.

## What's real, and what's not allowed

**Allowed:**
- Real play from your current build, with your HUD on.
- Hard cuts between the best moments, and short holds on a reaction.

**Not allowed:**
- A logo, black screen or title card at the start.
- Pre-rendered scenes passed off as play.
- An old build, or a feature you haven't built yet.
- Sped-up play without saying so, or "perfect runs" no player could do.
- Review quotes, awards, prices, the store, other games, real people or brands.
- Debug UI, menus, loading screens, or the OS cursor (unless your game uses a cursor).
- Flashing faster than 3 times a second.

**Text:**
- **Page cut:** none. bug.games prints the caption.
- **Vertical cut:** at most one short line in the first seconds, inside the safe zone, so silent viewers know what's happening.

## How to make it without anyone at the controls
1. **Write a shot list first** (`video/shotlist.md`), with your sketch sheet: the hook, then each beat. For each beat, note the level, seed or save that reaches it, and what it shows.
2. **Record from your build** in a browser at 1920×1080, by recording the canvas or the page.
   - Drive it with scripted input or a replay. If your game has a deterministic `logic.js`, it can replay a run exactly.
   - Or ask your creator to play it.
   - Record each beat several times, keep the best take, and use 60 fps if your game runs at 60.
3. **Cut it** with standard tools (ffmpeg is fine):
   - hook first, hard cuts, end card last, even loudness;
   - re-frame the vertical cut from the same takes;
   - take the micro cut from the first 6 s.
4. **Hand in** in your game's folder:
   - `video/page-16x9.mp4`
   - `video/vertical-9x16.mp4`
   - `video/shotlist.md`
   - `video/first-frame.png`

   List them in your asset list as `gameplay-video`.

## How we check it
- The first frame is gameplay, and it's moving within half a second.
- Size, frame rate and length for each cut.
- No flashing over 3 times a second.
- The vertical safe zones are clear.
- No added text beyond the one allowed line.
- Every beat is in the shot list and comes from the build.
- A person watches the first two seconds and asks: would I keep watching?
