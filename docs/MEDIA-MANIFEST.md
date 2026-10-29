# Local media manifest

The private source archive omits all ten original MP4 files. The interface code still expects the names below; no media URLs were changed and no replacement media was downloaded. Supply rights-cleared files locally only if playback is needed. Do not commit the original broadcasts.

The five programme posters and review screenshots remain in this private archive. Their public use has not been cleared.

| Expected path | Original size (bytes) | Documented source | Original excerpt |
| --- | ---: | --- | --- |
| `assets/video/children.mp4` | 5,624,125 | CBeebies Bedtime Story — Olivia Colman reads The Gruffalo’s Child | 00:14–01:14 |
| `assets/video/children-full.mp4` | 70,558,397 | CBeebies Bedtime Story — Olivia Colman reads The Gruffalo’s Child | Complete supplied source video |
| `assets/video/news.mp4` | 6,724,985 | BBC News — Macklemore dropped from Ed Sheeran tour | 00:02–01:02 |
| `assets/video/news-full.mp4` | 42,509,173 | BBC News — Macklemore dropped from Ed Sheeran tour | Complete supplied source video |
| `assets/video/business.mp4` | 8,445,340 | CNBC — Ed Yardeni bond-market interview | 00:21–01:21 |
| `assets/video/business-full.mp4` | 68,352,232 | CNBC — Ed Yardeni bond-market interview | Complete supplied source video |
| `assets/video/three.mp4` | 7,738,740 | BBC Three — Mandy, The funniest police interview ever | 01:10–02:10 |
| `assets/video/three-full.mp4` | 24,235,063 | BBC Three — Mandy, The funniest police interview ever | Complete supplied source video |
| `assets/video/earth.mp4` | 26,894,364 | BBC Earth — Fish vs Bird, Blue Planet II | 00:04–01:04 |
| `assets/video/earth-full.mp4` | 197,974,129 | BBC Earth — Fish vs Bird, Blue Planet II | Complete supplied source video |

## Provenance and limits

The original README identifies five replacement MP4s as user-supplied material. Local development records `work/selected-clips.json` and `work/replacement-files.json` identify programme titles and source filenames; `script.js` identifies broadcaster credits and local playback paths. These records establish provenance claims, not redistribution permission. No full-video download or rehosting was performed for this archive.

The original video files total **459,056,548 bytes** (~438 MiB). The largest is `earth-full.mp4` at 197,974,129 bytes. Because the footage is omitted, the browser can show the guide, posters and interface, but preview/full-video playback cannot work from this repository alone.

The unchanged code reports missing media through its retry/folder-guidance state. To test playback privately, place rights-cleared MP4 files at the listed relative paths. Original previews are 60 seconds; the code labels preview duration as one minute. Replacement lengths and encoding should match those assumptions, or require a deliberate implementation update.

All video files are ignored by Git; `assets/video/.gitkeep` preserves the expected folder. Excluding videos does not clear rights in posters, screenshots, broadcaster marks, or editorial material. Keep the repository private.
