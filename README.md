# Concosion

Stickman Concussion Adventure is a lightweight, single-page browser game built with
pure HTML/CSS/JavaScript. It is designed for easy GitHub Pages deployment and uses
arrow keys (plus optional number keys in the keypad puzzle) for all gameplay.

## Game Overview
- **Tone:** light, humorous, and kid-friendly.
- **Goal:** help NPCs to regain memories, unlocking abilities along the way.
- **Structure:** the game starts in a hospital room and can transition outside once
  the player remembers how to walk.

## Current MVP Flow
1. **Hospital intro:** the nurse walks to the stickman and starts a clear, real-worded
   conversation.
2. **Keypad puzzle:** a keypad overlay appears with a sticky note showing the code.
   Because of the concussion, the digits are scrambled when pressed.
   - Use **arrow keys** to move the keypad selector; moving onto a key presses it.
   - Use **number keys** to enter digits directly (the scrambled digit appears in the
     display).
   - The scrambled mapping is hidden in the UI so players must deduce it from inputs.
3. **Walking unlock:** after the correct code is entered, the stickman automatically
   stands up and gains movement control with the arrow keys.

## Controls
- **Arrow keys:** move the stickman once walking is unlocked; navigate the keypad.
- **Number keys:** enter digits during the keypad puzzle.

## Files
- `index.html` — single-page game (HTML, CSS, JS all embedded).
- `README.md` — this documentation.

## GitHub Pages
Deploy by serving the repo root. The game will be available at:
`https://aksharagummadi.github.io/concosion/`

## Development
To run locally:
```bash
python -m http.server 8000
```
Then open `http://127.0.0.1:8000/index.html`.
