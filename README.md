# Web Media Player

A responsive, single-file HTML + CSS + JavaScript media player for local audio and video files.

**Live demo:** https://abhijeet-kumar-prajapati.github.io/Web-Media-Player/

## Features

- Plays local video and audio files straight from your device (no upload, no server)
- Multi-file playlist with remove buttons and auto-advance
- Progress bar with click-to-seek and time display
- Volume and brightness controls
- Playback speed (0.25x - 2x)
- Bass boost indicator (visual)
- Fullscreen video
- Keyboard shortcuts

## Keyboard shortcuts

| Key | Action |
| --- | --- |
| `Space` | Play / Pause |
| `←` / `→` | Seek back / forward 5 seconds |
| `↑` / `↓` | Volume up / down |

## Files

| File | Purpose |
| --- | --- |
| `index.html` | The complete player (all CSS and JS is inline) |
| `player.html` | Redirect to `index.html`, kept so older links still work |

## Running locally

No build step and no dependencies. Just open `index.html` in a browser, or serve the folder:

```bash
python -m http.server 8000
```

Then visit http://localhost:8000

## Deploying to GitHub Pages

1. Create a repository and upload the files to the `main` branch.
2. Go to **Settings → Pages**.
3. Under **Source**, choose **Deploy from a branch**.
4. Select `main` and the `/ (root)` folder, then save.

> **Important:** the entry file **must** be named `index.html`. GitHub Pages serves
> `index.html` from the root. If it is missing, Pages falls back to rendering
> `README.md` and you will only see plain text.