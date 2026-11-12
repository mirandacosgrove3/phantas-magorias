# PHANTAS MAGORIAS

Minimal video-title player for iPad. Thin white text on black; tap a title to open a floating, movable, resizable player.

- **Load videos:** tap "tap to load videos" (or long-press empty space to add more). Videos stay on the device in Safari's site storage — nothing is uploaded.
- **Window:** drag to move, pinch or drag the corner to resize, tap to pause, × to close.
- **Layout:** new windows tile around each other; once you move/resize one, your layout is left alone and new windows go into the emptiest space.
- **Duplicates:** the same file can't be loaded twice; tapping an already-open title brings its window forward.
- **Sound on iPad:** iOS allows one video with sound at a time — all windows keep playing (no pausing), tap a window to give it the sound.
- **Titles:** the topmost window's title glows pink; when another window takes focus it reverse-types into a short line, and types back out when its window closes.
- **Fullscreen:** two-finger tap on empty space, or press F.
- **Spacebar:** closes everything and scrolls to top.
- **Local mode:** drop `index.html` in a folder with the videos listed in `MANIFEST` and they load automatically.

Edit `index.html` on github.com (press `.` for the editor); Pages redeploys on each commit.
