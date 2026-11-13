# PHANTAS MAGORIAS

Minimal video-title player for iPad. Thin white text on black; tap a title to open a floating, movable, resizable player.

- **Load videos:** tap "tap to load videos" (or long-press empty space to add more). Videos stay on the device in Safari's site storage — nothing is uploaded.
- **Window:** drag to move, pinch or drag the corner to resize, tap to pause, × to close.
- **Layout:** untouched windows open at a fixed size in whichever spot overlaps other windows and the title text the least (leaning top-right, avoiding text hardest); opening or closing one never moves the others. Once you move/resize one, new windows go into the emptiest space (also avoiding text).
- **Duplicates:** the same file can't be loaded twice; tapping an already-open title brings its window forward.
- **Sound on iPad:** iOS allows one video with sound at a time — all windows keep playing (no pausing), tap a window to give it the sound.
- **Audio lock:** hold a window still to lock the sound to it (thin glassy pink border). A small sound-wave appears left of its title, matching the title's line colour; tap the wave to unlock.
- **Titles:** the topmost window's title glows pink; when another window takes focus it reverse-types into a short line, and types back out when its window closes.
- **Rename:** tap-and-hold a title — it cuts itself away, a pink caret blinks, and a two-ring wheel rises in the bottom-right. Outer ring: letters, three per rounded segment (abc … yz). Inner greyish ring: numbers (123, 456, 789, 0). Spin either ring with one finger or tap a segment; the pink segment's characters show in the centre — tap one to place it. Corner pieces: pull-out keyboard (top-left), backspace (top-right), heart = kaomoji set (bottom-left), shift (bottom-right: tap = next letter, double-tap = caps lock). The pull-out keyboard is a plain grid (a–m / n–z) with a number row and an idle-scrolling kaomoji strip on top (touch to stop, drag to scroll, tap to place). Corner pieces follow the wheel's edge. Along the bottom centre of the screen: cancel (red), + videos, keyboard icon (raises the iPad's own keyboard), OK (turquoise).
- **Collapsed lines:** rainbow, one hue per line, a full spectrum every 12 lines, then it loops.
- **Reset:** two-finger tap on empty space (or spacebar) closes everything and scrolls to top.
- **Fullscreen:** three-finger tap on empty space, or press F.
- **Local mode:** drop `index.html` in a folder with the videos listed in `MANIFEST` and they load automatically.

Edit `index.html` on github.com (press `.` for the editor); Pages redeploys on each commit.

**After editing by hand, change the `BUILD` stamp in index.html** (any new value). The installed iPad app compares it against the live copy on launch and reloads itself when it differs.
