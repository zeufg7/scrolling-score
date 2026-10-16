# Scrolling Score

A scrolling sheet music viewer that stays in sync with an audio or video recording. Built for studying scores, live streams, and recording film-music analysis videos.

**Try it online:** https://zeufg7.github.io/scrolling-score/

Everything runs in your browser. Your files are never uploaded anywhere.

> The interface is currently in Brazilian Portuguese.

## Features

- **Reads MusicXML** (`.musicxml`, `.xml` and `.mxl`) exported from Cubase, Dorico, Sibelius or MuseScore.
- **Two scroll modes:** a continuous horizontal strip with a fixed playhead, or full systems scrolling vertically.
- **Notes light up** while they sound.
- **Sync to audio or video** (mp3, wav, m4a, mp4, mov, webm) through sync points. Between two points the score follows the recording's real tempo, including rubato and fermatas.
- **Timeline** showing video frames, the audio waveform and the score's bars on one time axis. Drag the score lane to line up the start, and drag any bar line to pin that bar to the right moment.
- **Tap to sync:** press play and hit `T` on each downbeat.
- **Multi-bar rests** from Dorico and Cubase are timed correctly.
- **Video export** as Horizontal 16:9 (YouTube), Vertical 9:16 (Shorts and TikTok) or Reels, with Instagram's safe areas kept clear.
- **Guide sound, metronome, practice loop** by bars, and playback speed from 40 to 150%.
- **Recording mode** that hides the interface, with dark, paper or chroma-green backgrounds for keying in OBS.

## How to use

1. Open the page and click **Abrir partitura** (Open score), or drag the file onto the window.
2. Click **Áudio / vídeo** and load the recording.
3. In the **timeline**, drag the score lane until the INÍCIO (start) marker lands where the music begins. If the tempo moves, pin more bars by dragging their bar lines, or press `T` on each downbeat while the music plays.
4. To make a video, click **Exportar** (Export) and pick a format. Recording happens in real time, so keep the tab open and visible until it finishes.

### Exporting your score as MusicXML

- **Cubase:** open the Score Editor, then File › Export › MusicXML.
- **Dorico:** File › Export › MusicXML.
- **MuseScore:** File › Export › MusicXML.

## Keyboard shortcuts

| Key | Action |
|---|---|
| Space | Play / pause |
| ← → | Previous / next bar |
| Home | Back to the start |
| T | Tap to sync (one tap per bar) |
| M | Pin the nearest bar to the current media time |
| , . | Fine-tune sync by 10 ms |
| K | Show / hide the timeline |
| H | Recording mode |
| F | Full screen |
| S C L | Guide sound, click, loop |
| [ ] | Loop start / end |
| + − | Score size |

## Running it locally

Download `index.html` and open it in Chrome or Edge. It needs an internet connection only to load its libraries and fonts.

Video export uses the browser's built-in recorder. Chrome and Edge on desktop produce MP4. Other browsers may produce WebM or not export at all.

## Credits

- Score engraving: [OpenSheetMusicDisplay](https://github.com/opensheetmusicdisplay/opensheetmusicdisplay) (BSD-3-Clause)
- `.mxl` reading: [JSZip](https://github.com/Stuk/jszip) (MIT)
- Fonts: Big Shoulders Display, IBM Plex Sans and IBM Plex Mono, via Google Fonts

Made by **Eliseu F. Guedes** · @o_zeufg

## License

MIT. See [LICENSE](LICENSE).
