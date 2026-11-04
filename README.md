# Backline

A backing track player that runs in the browser: mixer, MP3/WAV import and export, stems, a click track with its own output, project files, and a library of songs and show set lists.

The master has a limiter (LIMIT, on by default) that keeps it below -1 dB, in playback and in master exports. The button next to it adds up to +12 dB of output gain for playback, for outputs that sound quiet such as the left/right split. The Click and Tracks strips have the same kind of button for the click output.

Click settings, including Count-in (1 bar to start), belong to the browser, not to each song, and the click starts muted. The Tracks strip next to Click sends the track mix to the click output too, so players hear the song with the click. It needs a click output other than "Mixed with tracks".

Pressing Play says "Ready" on the click output, waits 3 seconds, then starts. Press Play or Stop during the wait to cancel. The voice follows the click's on/off button, mute and fader, so it is silent while the click is muted. It was made with the macOS Samantha voice.

Use Chrome or Edge to send the click to a separate output device. Audio stays on your computer and is never uploaded.

## Sharing on the web

The song and show list is saved in `library/index.json` in this repository. The audio is one `.btlib` file on Google Drive, shared with anyone who has the link. Use **Library > Publish list** to save the file and publish the list. Only share music you have the right to share.

To switch to a new library file, upload it to Drive, then use **Replace Drive file** in **Web library**. It can also rebuild the song and show list from the file.

To take something off the shared list, open **Library > Web library** and press **Delete** on a show or song. This needs a GitHub token too. It does not change your own library or the file on Google Drive.

Links: `?show=<id>`, `?song=<id>`, `?project=<url>`, `?library=<url to index.json>`

## Third-party code

`index.html` includes the minified build of [lamejs](https://github.com/zhuker/lamejs) 1.2.1 for MP3 encoding, licensed under the LGPL-3.0. Its source is available at that link.
