# ZMK Configuration

ZMK configuration for [charybdis](https://github.com/Bastardkb/Charybdis/tree/main) wireless
version with [nice!nano](https://nicekeyboards.com/nice-nano/).

## Ergonomic defaults

The base layer keeps the Pointer layer on a left lower thumb key so it can be
held while operating the right-hand trackball. The left thumb cluster provides
**GUI/Command**, **Space**, **Num**, **Pointer**, and **Left Alt/Option**; the
right thumb cluster provides **Sym**, **Enter**, and Right Alt/AltGr.

The left outer home and bottom keys provide dedicated **Left Shift** and
**Left Control**. No base-layer modifier uses hold-tap timing. Caps Lock
remains available as **Func + G**.

## Keymap

[![Charybdis keymap](keymap-drawer/charybdis.svg)](keymap-drawer/charybdis.svg)

## Layer and shortcut guide

Layer keys are momentary unless noted otherwise: hold the listed key while
pressing another key.

| Layer | How to activate | Highlights |
| --- | --- | --- |
| **Num** | Hold the left **Num** thumb key | Left-hand numeric pad, editing keys, and F1–F12 |
| **Sym** | Hold the right **Sym** thumb key | Complete programming punctuation set, Backspace, and Delete |
| **Func** | Hold **Num + Sym** together | Bluetooth, USB, media, RGB, function keys, Caps Lock, Game, and Studio controls |
| **Pointer** | Hold the lower-left **Pointer** thumb key | Mirrored mouse buttons and arrow keys, plus access to Scroll and Snipe |
| **Scroll** | Hold **Pointer + Z** | The trackball and right directional keys scroll horizontally and vertically at reduced speed; the left directional keys remain arrows |
| **Snipe** | Chord **Pointer + Z + X** within 75 ms and hold Z+X | Precision trackball movement and arrow keys |
| **Game** | Hold **Func**, then tap **B** | Locks the gaming layer on; tap either the **Num** or **Sym** thumb key to return to Base |

### Developer symbols

The Sym layer follows the shifted number row and groups matching delimiters and
operators together. Its unused outer-column keys are transparent, preserving
Base-layer Escape, Tab, Shift, Control, Backspace, backslash, apostrophe, and
grave access.

| Positions | Symbols |
| --- | --- |
| Number row | `! @ # $ %` · `^ & * ( )` |
| Q–T | `` ` ~ < > ? `` |
| Y–P | `- = [ ] \` |
| A–G | `; : ' " /` |
| H–Semicolon | `_ + { } \|` |
| V / B | Backspace / Delete |

This covers the standard US programming punctuation set, including both kinds
of brackets, braces, parentheses, quotes, slashes, comparison characters, and
the common arithmetic and logical symbols.

### Numeric pad and function keys

The Num layer places a conventional numeric-pad pattern on the left and keeps
all function keys on the right:

```text
7 8 9 / Backspace    F1  F2  F3  F4  F5  F6
4 5 6 * =            F7  F8  F9  F10 F11 F12
1 2 3 - ,
0 . Enter + Delete
```

### Function, Bluetooth, and media shortcuts

| Action | Combination |
| --- | --- |
| Use Bluetooth output | **Func + H** |
| Select Bluetooth profile 0 | **Func + J** |
| Select Bluetooth profile 1 | **Func + K** |
| Use USB output | **Func + N** |
| Caps Lock | **Func + G** |
| Mute | **Func + A** |
| Volume down | **Func + S** |
| Volume up | **Func + D** |
| F1–F6 | **Func + Q–Y** |

Select an unused Bluetooth profile before pairing a new host. Selecting a
profile switches hosts; it does not clear an existing bond.

### RGB underglow

| Action | Combination |
| --- | --- |
| Toggle underglow | **Func + Left Control** |
| Next effect (Solid → Breathe → Spectrum → Swirl) | **Func + Backspace** |
| Increase brightness | **Func + Backslash** |
| Decrease brightness | **Func + Apostrophe** |

### Pointer controls and key combos

The trackball normally moves the pointer. While holding **Pointer**, use either
**F/E/S** or **J/I/L** for left/middle/right click. On **Pointer**, **Snipe**,
and **Scroll**, the left-hand **D/X/C/V** diamond acts as Up/Left/Down/Right.
The right-hand **K/M/Comma/Period** diamond acts as arrows on **Pointer** and
**Snipe**, and scrolls Up/Left/Down/Right on **Scroll**.

On Pointer, hold **Z** to scroll. Press **Z + X** together within 75 ms and
hold both keys for Snipe. Release the keys and the keyboard returns to Pointer.

These Base-layer two-key combos can be pressed simultaneously:

| Keys | Result |
| --- | --- |
| **Z + X** | Left Shift |
| **X + C** | Left Alt/Option |
| **F + G** | Left Control |
| **H + J** | Right Control |
| **Comma + Period** | Left Alt/Option |

## ZMK Studio

ZMK Studio is enabled for both the right-half central and dongle firmware
builds. Connect whichever one is acting as the central device over USB. Studio
locking is disabled, so Studio can edit the keymap immediately without an
unlock key combination.
