# Falling Notes

A LUNA Add On that shows MIDI notes falling onto a piano keyboard in time with LUNA, and
teaches you to play the piano. It has two modes, picked at the top left:

- **Display** shows your session's MIDI tracks falling onto the keys as LUNA plays. Click the
  keys to play into the tracks, scroll to scrub, and edit the notes piano-roll style while
  stopped.
- **Learn** opens a lesson session of its own, so your work is never touched. It has piano
  lessons from Beginner to Late Elementary, with finger numbers, the music written out on a
  grand staff, practice at a slower tempo that steps up as you get it right, and tests that
  score your playing on any MIDI keyboard.

Requires LUNA 3.1.2 or later. Learn uses UA's Shape instrument (House Piano preset) for its
piano.

## Install

1. Download `falling-notes.lunaaddon` from the latest release on this repository's
   **Releases** page.
2. Double-click the file. LUNA installs it into its Add Ons folder.

To update, install the newer `.lunaaddon` the same way.

## Display

Choose **Add Ons > Windows > Falling Notes**. The window follows LUNA's playhead: play, stop,
seek or loop in LUNA and the notes follow. A key lights while its note sounds. Falling Notes
sends no MIDI during playback; LUNA plays the tracks as usual.

- **Tracks**: check the MIDI tracks to show, any number of them (**All** and **None** are at
  the foot of the list). Every MIDI track shows until you choose. Notes take their track's
  color; brighter notes are louder. Muted clips and muted notes are left out.
- **BPM**: the tempo at the playhead. Type a value or use **−** and **+** (Shift: 5 BPM) to
  change the session's tempo there, as LUNA's own tempo field does.
- **Click**: LUNA's metronome on or off.
- **Grid**: what edits and clicks in the overview snap to. The button turns snapping off.
- **Overview**: the strip under the keyboard shows every note of the checked tracks across the
  session. Click or drag in it to move the playhead.

Notes fall at a steady speed, even across tempo changes.

### Play

Click a key to play its note into every checked track, as a MIDI keyboard would. Lower on the
key is louder. Drag across the keys for a glissando. A record-enabled track records what you
play.

While LUNA is stopped, the mouse wheel or trackpad scrubs: the playhead moves with your
fingers, and the notes play as they cross the top of the keyboard.

### Edit

While LUNA is stopped, the field is a piano roll:

- Click a note to select it and hear it; Shift-click adds or removes it.
- Drag a note to move it in time and pitch, or drag either end to trim it.
- Drag on empty space to select with a box.
- Double-click empty space to add a note, one grid step long. With more than one track
  checked, **Edit** chooses which track gets it.
- Delete or Backspace deletes the selection; Cmd+A selects all; Escape deselects.

Each edit is one undo step in LUNA. Editing turns LUNA's **Link Edit & Play** off so the
playhead stays put; the ⚙ menu has a button to turn it back on.

## Learn

Choosing **Learn** asks first, then closes your session and opens the lesson session, with a
piano track playing Shape's House Piano. Choosing **Display** closes the lesson session and
brings your session back.

- **Lessons**: pick a lesson by level: **Beginner**, **Elementary** and **Late Elementary**,
  from finding middle C to scales in more keys, chords, accompaniment patterns and short
  pieces. The lesson's name and goal show over the notes. Loading a lesson replaces the notes
  on the lesson track; LUNA's undo brings the old ones back.
- **Fingering**: each falling note carries a finger number, 1 for the thumb to 5 for the
  little finger, light for the right hand and dark for the left. The ⚙ menu turns the numbers
  off and opens a diagram of both hands with the lesson's starting position.
- **Notation**: the strip under the keyboard shows the lesson on a grand staff, with the
  fingering, sliding past a fixed playhead. Click a note to move there; drag to move the music.
- **Practice** (▶): plays the lesson at the practice tempo without changing the session's
  tempo. Each lesson starts at about 70% of its target tempo, which shows beside the practice
  tempo. Change the practice tempo with **−** and **+** (4 BPM; Shift: 1) or type it.
- **Test**: with Test on, ▶ counts you in for a bar, then listens to every MIDI keyboard (and
  the on-screen keys) instead of playing. Each note is scored on being played on time and held
  for its length; a late note counts for half. At the end you get a score and your hits,
  misses, notes held short, late notes and extra notes. A perfect run sets the next run 4 BPM
  faster, up to the target; a perfect run at the target offers the next lesson.
- **Click**: a click on the beats during practice and tests.

## Settings

The ⚙ menu holds **Lookahead** (how many seconds of music show above the keyboard),
**Keyboard** (fit the keyboard to the notes, or show all 88 keys; Learn always shows 88), and
the fingering and Link Edit & Play buttons.

Your choices (tracks, settings, practice tempo, the last lesson) are saved with the session,
outside LUNA's undo history. A new session starts from your last settings.
