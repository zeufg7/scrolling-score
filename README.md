# Scrolling Score

A scrolling sheet music viewer that stays in sync with an audio or video recording. Built for studying scores, live streams, and recording film-music analysis videos.

**Try it online:** https://zeufg7.github.io/scrolling-score/

Everything runs in your browser. Your files are never uploaded anywhere.

> The interface is currently in Brazilian Portuguese.

## Features

- **Reads MusicXML** (`.musicxml`, `.xml` and `.mxl`) exported from Cubase, Dorico, Sibelius or MuseScore.
- **Reads PDF scores too.** The app finds each system on the pages and proposes crops you can move, resize, delete or draw by hand. The crops are stitched into one continuous strip, aligned on the staff and scaled to a common staff size. Bar lines are detected automatically (stems, time signatures and bar numbers are told apart from real bar lines) and you can add, move or remove them, and say how many bars a multi-bar rest is worth. The PDF and your crops are kept in the browser and reopen with the page.
- **Mark up PDF scores:** click **Editar** on a PDF to get an eraser (drag over anything to hide it; select the erased area and delete it to bring it back), a pencil, text boxes with an optional frame for rehearsal marks, and slurs and ties you drag from one note to another. Slurs and ties can be bent, flipped above or below and moved, which fixes slurs that break badly at the end of a line once the systems are joined. Everything you draw is saved with the PDF project and shows in exported videos.
- **Repeats and jumps:** the score is played in performance order, not written order. Repeat signs, 1st/2nd/3rd endings, Segno, To Coda, Coda, Fine, D.C., D.C. al Coda, D.C. al Fine, D.S., D.S. al Coda and D.S. al Fine are read from MusicXML automatically. For PDFs, or to fix a file, open **Saltos** in the timeline, pick a symbol from the palette and click the bar, either in the timeline or on the score. The timeline shows every pass of every bar, so you can pin the 2nd time through a passage to the video like any other bar. The video itself is never cut or moved. For live versions that don't follow the page, type your own order (for example `1-59, 52-58, 60-142`).
- **Engraving fonts:** notes, clefs, rests and accidentals can be drawn in Finale Maestro (the default), Engraver, Legacy, or the handwritten Broadway, Jazz and Ash, all from MakeMusic. Chord symbols are set in Arial Bold with Maestro sharps and flats, the same style Dorico uses, and dynamics use the matching music font. Choose under Ajustes › Fonte musical, where you can also make the symbols and the noteheads bigger without changing the staff size. Exported videos keep the same fonts.
- **Two scroll modes:** a continuous horizontal strip with a fixed playhead, or full systems scrolling vertically.
- **Notes light up** while they sound.
- **Sync to audio or video** (mp3, wav, m4a, mp4, mov, webm) through sync points. Between two points the score follows the recording's real tempo, including rubato and fermatas.
- **Timeline** showing video frames, the audio waveform and the score's bars on one time axis. Drag the score lane to line up the start, and drag any bar line to pin that bar to the right moment.
- **Tap to sync:** press play and hit `T` on each downbeat.
- **Multicam (up to 4 cameras):** add videos of the same performance and each one is lined up with the main audio automatically by comparing their sound (about 1 ms precision). Fine-tune by dragging a camera's lane in the timeline. Any camera can provide the main audio.
- **Counts rest bars:** during multi-bar rests the reading line steps through each bar of the rest and only moves on when the music comes back. Multi-bar rests from Dorico and Cubase are timed correctly.
- **Sticky clef, key and time signature** stay pinned at the left edge while the score scrolls and change with the music: when a staff switches clef, or the key or time signature changes, the pinned header shows the new one from that point on. They stay pinned together with the piano brace and the choir bracket, in the app and in exported videos. When a MusicXML file defines no groups, parts with one staff each that sit together (a choir, for example) get a bracket automatically.
- **Video export** as Horizontal 16:9 (YouTube), Vertical 9:16 (Shorts and TikTok) or Reels, with Instagram's safe areas kept clear. A live preview lets you set the score size and position, the band height and the video size before recording. With cameras loaded, the preview becomes a layout composer: pick a preset (grid with the score across the middle, side by side, or main camera plus smaller ones) and drag or resize every camera and the score band, with snapping to edges, centre and neighbouring boxes.
- **Separate layers for your editor:** record everything together, cameras only (synced, with audio), or the score only on green or black. Separate exports of the same range start at the same instant and have the same length, so in CapCut or any editor you stack them at zero and key out the green.
- **Score editing:** click any note, rest, dynamic, hairpin, slur or text to select it, then change pitch, duration, articulations, stems and dynamics, turn notes into rests, add hairpins, edit texts and tempo marks. Move dynamics, texts, hairpins and slurs above or below the staff, or drag them anywhere (saved as standard MusicXML offsets). Undo/redo, and save the edited MusicXML.
- **Adjustable reading line:** height, thickness and position.
- **Guide sound, metronome, practice loop** by bars, and playback speed from 40 to 150%.
- **Recording mode** that hides the interface, with dark, paper or chroma-green backgrounds for keying in OBS.

## How to use

1. Open the page and click **Abrir partitura** (Open score), or drag the file onto the window. For a PDF, follow the three steps: crop the systems, check the bar lines, set the time signature and starting tempo. To adjust a PDF later, click **Editar**.
2. Click **Áudio / vídeo** and load the recording.
3. In the **timeline**, drag the score lane until the INÍCIO (start) marker lands where the music begins. If the tempo moves, pin more bars by dragging their bar lines, or press `T` on each downbeat while the music plays.
4. If the piece has repeats, endings, D.C. or D.S., check the order under **Saltos** in the timeline. Add or remove symbols by choosing one and clicking a bar, or type the order by hand.
5. For a multicam video, click **+ Câmeras** in the timeline (or Ajustes › Câmeras) and add up to four videos. They sync themselves to the main audio.
6. To make a video, click **Exportar** (Export). Pick a format, adjust the framing in the preview, then click **Gravar vídeo** (Record video). Recording happens in real time, so keep the tab open and visible until it finishes.
7. To fix the score, click **Editar** (Edit), select an item and use the bar that appears at the top. Save with **Salvar MusicXML**.

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

### In edit mode

| Key | Action |
|---|---|
| ↑ ↓ | Semitone up / down |
| Ctrl + ↑ ↓ | Octave up / down |
| ← → | Previous / next note |
| 7 6 5 4 3 | Whole, half, quarter, eighth, 16th (Dorico style) |
| . | Toggle dot |
| ↑ ↓ ← → on a mark | Move it 1 px (Shift: 10 px) |
| Delete | Turn note into rest / delete mark |
| Ctrl + Z / Ctrl + Y | Undo / redo |
| Ctrl + S | Save MusicXML |
| Esc | Deselect / leave edit mode / drop the jump symbol in hand |

## Running it locally

Download `index.html` and open it in Chrome or Edge. It needs an internet connection only to load its libraries and fonts.

Video export uses the browser's built-in recorder. Chrome and Edge on desktop produce MP4. Other browsers may produce WebM or not export at all.

## Credits

- Score engraving: [OpenSheetMusicDisplay](https://github.com/opensheetmusicdisplay/opensheetmusicdisplay) (BSD-3-Clause)
- `.mxl` reading: [JSZip](https://github.com/Stuk/jszip) (MIT)
- PDF rendering: [PDF.js](https://github.com/mozilla/pdf.js) (Apache-2.0)
- Fonts: Big Shoulders Display, IBM Plex Sans and IBM Plex Mono, via Google Fonts
- Music fonts: Finale Maestro, Maestro Text, Engraver, Legacy, Broadway, Jazz and Ash by MakeMusic, Inc., under the SIL Open Font License 1.1 (see [fonts/MakeMusic-OFL.txt](fonts/MakeMusic-OFL.txt)). Glyph outlines are converted and subset for use in this app.

Made by **Eliseu F. Guedes** · @o_zeufg

## License

MIT. See [LICENSE](LICENSE).
