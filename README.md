# PHANTAS MAGORIAS

Minimal video-title player for iPad. Thin white text on black; tap a title to open a floating, movable, resizable player.

- **Load videos:** tap "tap to load videos" (or long-press empty space to add more). Videos stay on the device in Safari's site storage — nothing is uploaded.
- **Window:** drag to move, pinch or drag the corner to resize, tap to pause, × to close.
- **Layout:** untouched windows open at a fixed size in whichever spot overlaps other windows and the title text the least (leaning top-right, avoiding text hardest); opening or closing one never moves the others. Once you move/resize one, new windows go into the emptiest space (also avoiding text).
- **Duplicates:** the same file can't be loaded twice; tapping an already-open title brings its window forward.
- **Sound on iPad:** iOS allows one video with sound at a time — all windows keep playing (no pausing), tap a window to give it the sound.
- **Audio lock:** hold a window still to lock the sound to it (thin glassy pink border). A small sound-wave appears left of its title, matching the title's line colour; tap the wave to unlock.
- **Titles:** the topmost window's title glows pink; when another window takes focus it reverse-types into a short line, and types back out when its window closes.
- **Databases:** the folder icon in the bottom row (while renaming) opens your databases — separate video lists, each with its own titles. With only one, it goes straight to naming a new one; otherwise tap a name to switch (current in pink, with its video count), hold a name to rename it, or + for a new one. A video used in several databases is stored once.
- **Rename:** tap-and-hold a title — it cuts itself away, a pink caret blinks, and a two-ring wheel rises in the bottom-right. Outer ring: letters, three per rounded segment (abc … yz). Inner greyish ring: numbers (123, 456, 789, 0). Spin either ring with one finger or tap a segment; the pink segment's characters show in the centre — tap one to place it. Corner pieces: a thin pull tab (top-left) — pull it up-left (or tap) and a full keyboard unfolds out of the corner and takes over the bottom of the screen (the wheel steps aside): a uniform 10-wide grid running edge to edge: kaomoji strip (touch to stop, drag to scroll, tap to place) with redo and backspace, number row, QWERTY with a teal OK after l, and shift … m, + videos, red cancel. The bottom control row hides while it's out. Its own top-left handle folds it back into the wheel (tap, or push it down-right). Top-right is split: redo (upper half) and backspace (half nearer the hand). Heart = kaomoji set (bottom-left), shift (bottom-right: tap = next letter, double-tap = caps lock). Corner pieces follow the wheel's edge. Along the bottom centre of the screen: cancel (red), + videos, keyboard icon (raises the iPad's own keyboard), OK (turquoise).
- **Collapsed lines:** rainbow, one hue per line, a full spectrum every 12 lines, then it loops.
- **Reset:** two-finger tap on empty space (or spacebar) closes everything and scrolls to top.
- **Fullscreen:** three-finger tap on empty space, or press F.
- **Local mode:** drop `index.html` in a folder with the videos listed in `MANIFEST` and they load automatically.

Edit `index.html` on github.com (press `.` for the editor); Pages redeploys on each commit.

**After editing by hand, change the `BUILD` stamp in index.html** (any new value). The installed iPad app compares it against the live copy on launch and reloads itself when it differs.

## Hold menu (crop / trim / sound)
Hold a playing window: three bubbles pop out around your finger. Drag onto one and let go, or let go in the middle and tap one.
- **top - sound**: locks the audio to that window (pink border). Pick it again to unlock.
- **bottom-left - crop**: full-screen editor. Drag the box or its pink corners; free, 1:1, 4:5, 16:9, 9:16, reset.
- **bottom-right - trim**: full-screen editor. Drag the pink start/end handles, drag the middle to slide the range, tap to scrub.
Crop and trim are saved per database item, so the same video can be cut differently in different databases.
Trim suggestions: the trim editor scans the start and end of the video and marks suggested cuts right on the timeline (red hatching plus a chip): an end card such as Instagram's logo/username outro (found as the last hard change in the final few seconds, so it fits each file), plus black lead-ins and fades to black. Tap a chip to apply it.
Playback modes: pull out the trim (scissors) bubble, then keep going up to the play bubble that sprouts from it (or tap trim once, then tap play). Modes: normal, boomerang, slo-mo boomerang, duo (fast rewind), echo, long exposure, slo-mo, fast, reverse. Boomerang/duo/reverse record one pass of the clip (trim range, a few seconds max) and play it back and forth, so trim first to choose the moment. Saved per database item.
Universal adjustments (Saturn icon in the bottom bar while renaming): per-database settings that layer over every video's own edits: auto-cut end cards / black starts, max length, same crop ratio, corners, same playback mode, filter look + brightness/contrast/saturation/hue, and blend mode. Live preview; cancel reverts.
Focus: holding a video lights it with a prism halo and dims the rest; letting go removes the bubbles but keeps the focus until you tap elsewhere.
Title hold menu (Y shape): up-left Aa = rename (wheel keyboard etc.), up-right planet = universal adjustments, with branches off the planet: camera (video manager) above-right, folder (databases) to the right. Near edges the shape slides inward instead of flipping.
Video manager: every stored video with size, length, resolution, which databases use it, its edits and whether it's open; add/remove from the current list; delete for good (tap twice); per-file save progress while importing; storage used/free and a "keep them" button that asks Safari not to clear the cache.
Universal: "tidy up now" (arrange) lays the open videos out once in rows that fill the screen at each video's own shape (no cropping). Auto-cut scans are saved per video and run in the background for the whole list (and new imports) while a cut toggle is on, so new videos are treated the moment they open.
The rename bar is now just cancel / iPad keyboard / OK; + videos, databases and the planet live in the title hold menu.
Universal also has "open all" (opens every video in the list one after another) and "cut off start / cut off end" (a strict number of seconds shaved off every video).
Memory manager (gauge, branching off the planet below the folder): live fps and stutters, decoding load, estimated video memory; open videos heaviest first with their effects and a close button; playback effects grouped; universal features costed; storage; and tips for what would help most.
