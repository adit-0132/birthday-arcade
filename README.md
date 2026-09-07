# birthday-arcade

A single-page 8-bit birthday arcade game. Three levels, one meter, no build step.

**Play it:** https://adit-0132.github.io/birthday-arcade/

## The levels

1. **The SF90** — 3x3 sliding-block puzzle over a photograph of a red Ferrari.
   Scrambled with legal moves only, so every board is solvable.
2. **The YC Startup** — rotate the pipes to connect *Sequoia / VC Bank* to
   *Your Startup*. A path is carved before the decoys are placed, so every
   grid has a solution. Connect it and the valuation flows.
3. **The College Dropout** — a Frogger-style escape from JIIT Sector 62.
   Dodge 70% attendance, T1, T2, an extremely fast T3, and heavy major
   projects; squeeze through the *40 Minimum Marks* gate. Past the gate you
   respawn at the checkpoint instead of the bottom.

Clear all three and the meter overloads.

## Controls

- Arrow keys / WASD to move in level 3 (on-screen D-pad on touch devices)
- Mouse to click tiles and pipes
- `M` or the `BGM` button to mute the music

## Tech

One file, no dependencies, no build. Vanilla HTML/CSS/JS, `Press Start 2P`
from Google Fonts, canvas for level 3, SVG for the meter, WebAudio for the
sound effects. Runs straight off the filesystem.

Background music: *Slow Jamz*. Drop any `bgm.mp3` next to `index.html` to
swap the track. If no track loads, the game synthesises its own 68bpm slow
jam in WebAudio as a fallback.
