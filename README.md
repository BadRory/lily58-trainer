# Lily58 Touch-Type Trainer

A keybr-style typing trainer for relearning touch typing on a Lily58 split keyboard. One HTML file. No install, no build, no server.

## Run it

Open `index.html` in a browser:

```sh
open index.html
```

## Features

- On-screen Lily58 layout that matches my ZMK keymap
- Next key lights up; green on hit, red on miss
- Names the finger to use for each key (for example "Left middle -> d")
- Resting-hands panel showing which keys each finger owns
- Starts with a few keys and unlocks a new letter after a clean, fast round
- Weak keys are drilled more often; per-key accuracy grid
- WPM, accuracy, streak and best WPM, saved in the browser (`localStorage`)
- Modes: letter drills, common words, home row

## Keymap

The layout is defined by the `LEFT` and `RIGHT` arrays near the top of the script in `index.html`. Each key is `[label, character, classes]`. The finger is set by an `f-..` class (`f-lp` is left pinky, `f-ri` is right index, `f-th` is thumb). Edit those to match your own board.

## Notes

- Base layer is QWERTY. Layer keys and modifiers are shown but not trained.
- Progress lives in your browser only. "Reset progress" clears it.
