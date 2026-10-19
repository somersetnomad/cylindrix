# Cylindrix

A falling-block puzzle game on a see-through drum.

The well is a cylinder of 12 columns. There are no walls: a ring clears only when all 12 cells around the drum are filled. Your piece always sits at the front, and moving it turns the drum. Blocks on the back show faintly through the glass, so you can always see the whole ring.

## How it plays

- **Growing pieces.** You start with the 2 trominoes (3 cells). After 8 rings, the 7 tetrominoes arrive, and after 30 rings, the 18 pentominoes. A program generates every shape by growing polyominoes one cell at a time and keeping one of each up to rotation.
- **Fair shuffles.** Each piece size has its own shuffled bag, so you see every shape once before any repeats.
- **Triangular scoring.** Clearing *k* rings at once scores T(*k*) × 100 × level, where T(*k*) = *k*(*k*+1)/2. The formula updates live on screen.
- **Hold.** Keep one piece aside and swap it in later, once per piece.
- **Two modes.** In Classic, the drum turns only when you move. In Drift, it also turns by itself on a timer that speeds up each level, reversing direction at every level change.
- **Demo.** A 30-second self-playing demo explains each rule as it happens.

## Controls

| Key | Action |
| --- | --- |
| ← → | Turn the drum |
| ↑ or X | Rotate clockwise |
| Z | Rotate anticlockwise |
| C or Shift | Hold or swap |
| ↓ | Soft drop |
| Space | Hard drop |
| P or Esc | Pause |

On phones, use the buttons under the board.

## Running it

The whole game is one file, `index.html`, with no build step or dependencies beyond Google Fonts. Open it in a browser, or serve the folder with any static host.
