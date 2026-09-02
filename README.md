# ZMK Configuration

ZMK configuration for [charybdis](https://github.com/Bastardkb/Charybdis/tree/main) wireless
version with [nice!nano](https://nicekeyboards.com/nice-nano/).

## Ergonomic defaults

The base layer keeps the pointer and scroll layers on the left lower thumb
keys, so they can be held while operating the right-hand trackball. The left
thumb cluster provides **Shift**, **Num**, and **Space**; the right thumb
cluster provides **Sym** and **Enter**. Right Control is on the remaining
right thumb key for common editor shortcuts.

## ZMK Studio

ZMK Studio is enabled on the right half, which is the split central. Flash the
`charybdis_right` firmware, then connect that half to the computer over USB.
To unlock Studio from the base layer, hold the left **Num** thumb key, hold the
right **Sym** thumb key (which becomes the Func layer key), and tap the right
**Enter** thumb key. The `studio-rpc-usb-uart` build snippet is already applied
to the right-half build in `build.yaml`.


