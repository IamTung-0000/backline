# Backline

A backing track player that runs in the browser: mixer, MP3/WAV import and export, stems, a click track with its own output, project files, and a library of songs and show set lists.

Use Chrome or Edge to send the click to a separate output device. Audio stays on your computer and is never uploaded.

## Sharing on the web

**Library > Publish to GitHub** puts the songs and shows you select in the `library/` folder of this repository. Everyone can then open them from **Library > Web library** or a shared link. Published audio is public, so publish only music you have the right to share.

Links: `?show=<id>`, `?song=<id>`, `?project=<url>`, `?library=<url to index.json>`

## Third-party code

`index.html` includes the minified build of [lamejs](https://github.com/zhuker/lamejs) 1.2.1 for MP3 encoding, licensed under the LGPL-3.0. Its source is available at that link.
