# Morse Trainer

A Flipper Zero game that teaches Morse code from zero through 13 progressive levels.

![icon](icon.png)

## Features

- **Three training modes** with independent progress: **Encoding** (you key the Morse), **Decoding** (you identify what you hear), and **Mixed**
- **13-level curriculum** ordered by symbol simplicity — from E/T up to full alphabet, digits, and callsign-style words
- **Challenge levels** every few levels: spell real words drawn from a rotating vocabulary pool
- **Free Practice mode**: key anything, the app decodes it live; play it back with Up
- **Adaptive review**: letters you keep missing show up more often
- **Real keying feel**: hold-to-key with live sidetone (speaker + LED), a visual dot/dash threshold bar, and Farnsworth-spaced playback for beginners
- **Hints**: 50/50 on multiple choice (Down) or a letter reference card while encoding (Up) — 2 per level
- Stars per level (80% = ★, 90% = ★★, perfect = ★★★), daily streak, lifetime stats
- Everything configurable: sound, vibration, letter gaps, pattern visuals, LED

## Controls

### Encoding questions
| Key | Action |
|-----|--------|
| OK (short hold) | dot |
| OK (long hold, past the bar's tick mark) | dash |
| *pause* | commits the letter |
| Left | clear current attempt |
| Up | letter hint (costs a hint) |

### Decoding questions
| Key | Action |
|-----|--------|
| Left / Right | select answer (wraps around) |
| OK | confirm |
| Up | replay audio |
| Down | 50/50 hint (costs a hint) |

Back twice abandons a level. Progress is saved to SD (`apps_data/morse_trainer/`) after every run.

## Requirements

No extra hardware — uses the built-in speaker, vibro motor, and LED.

## Building

Built with [ufbt](https://github.com/flipperdevices/flipperzero-ufbt):

```
ufbt launch
```
