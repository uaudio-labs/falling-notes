# Falling Notes

A LUNA Add On that shows your MIDI tracks' notes falling onto a piano keyboard, in time with
LUNA's playhead. Click the keys to play notes into the tracks.

Requires LUNA 3.1.2 or later.

## Install

1. Download `falling-notes.lunaaddon` from the latest release on this repository's
   **Releases** page.
2. Double-click the file. LUNA installs it into its Add Ons folder.

To update, install the newer `.lunaaddon` the same way.

## Use

Choose **Add Ons > Windows > Falling Notes**. The window opens with the session and follows
LUNA's playhead: play, stop, seek or loop in LUNA and the notes follow. A key lights while its
note sounds. Falling Notes sends no MIDI during playback; LUNA plays the tracks as usual.

- **Tracks**: check the MIDI tracks to show, any number of them (**All** and **None** are at
  the foot of the list). Every MIDI track shows until you choose. Your choice is saved with the
  session. Notes take their track's color; brighter notes are louder.
- **Lookahead**: how many seconds of music show above the keyboard.
- **Keyboard**: fit the keyboard to the notes, or show all 88 keys.

Notes fall at a steady speed, even across tempo changes. Muted clips and muted notes are left
out.

### Play

Click a key to play its note into every checked track, as a MIDI keyboard would. Lower on the
key is louder. Drag across the keys for a glissando. A record-enabled track records what you
play.
