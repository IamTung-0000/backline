# Backline

A backing track player that runs in the browser: mixer, MP3/WAV import and export, stems, a click track with its own output, project files, and a library of songs and show set lists.

Use Chrome or Edge to send the click to a separate output device. Audio stays on your computer and is never uploaded.

## Sharing on the web

The song and show list is saved in `library/index.json` in this repository. The audio is one `.btlib` file on Google Drive, shared with anyone who has the link. Use **Library > Publish list** to save the file and publish the list. Only share music you have the right to share.

To take something off the shared list, open **Library > Web library** and press **Delete** on a show or song. This needs a GitHub token too. It does not change your own library or the file on Google Drive.

Links: `?show=<id>`, `?song=<id>`, `?project=<url>`, `?library=<url to index.json>`

## Third-party code

`index.html` includes the minified build of [lamejs](https://github.com/zhuker/lamejs) 1.2.1 for MP3 encoding, licensed under the LGPL-3.0. Its source is available at that link.
