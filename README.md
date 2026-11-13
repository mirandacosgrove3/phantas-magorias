# PHANTAS MAGORIAS

Minimal video-title player for iPad. Thin white text on black; tap a title to open a floating, movable, resizable player.

- **Load videos:** tap "tap to load videos" (or long-press empty space to add more). Videos stay on the device in Safari's site storage — nothing is uploaded.
- **Window:** drag to move, pinch or drag the corner to resize, tap to pause, × to close.
- **Layout:** untouched windows open at a fixed size in whichever spot overlaps other windows and the title text the least (leaning top-right, avoiding text hardest); opening or closing one never moves the others. Once you move/resize one, new windows go into the emptiest space (also avoiding text).
- **Duplicates:** the same file can't be loaded twice; tapping an already-open title brings its window forward.
- **Sound on iPad:** iOS allows one video with sound at a time — all windows keep playing (no pausing), tap a window to give it the sound.
- **Titles:** the topmost window's title glows pink; when another window takes focus it reverse-types into a short line, and types back out when its window closes.
- **Rename:** tap-and-hold a title — it cuts itself away, a pink caret blinks, and a type-sheet keyboard slides up (kaomoji by category on the right, red cancel, + add videos, turquoise enter). Keys fire on release, so sliding a finger never types. The file type always stays. Titles are saved on the device.
- **Collapsed lines:** rainbow, one hue per line, a full spectrum every 12 lines, then it loops.
- **Reset:** two-finger tap on empty space (or spacebar) closes everything and scrolls to top.
- **Fullscreen:** three-finger tap on empty space, or press F.
- **Local mode:** drop `index.html` in a folder with the videos listed in `MANIFEST` and they load automatically.

Edit `index.html` on github.com (press `.` for the editor); Pages redeploys on each commit.

**After editing by hand, change the `BUILD` stamp in index.html** (any new value). The installed iPad app compares it against the live copy on launch and reloads itself when it differs.
