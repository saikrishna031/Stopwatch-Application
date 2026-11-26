# Project 05 — Chrono Stopwatch

A responsive stopwatch built with HTML5, CSS3 and Vanilla JavaScript. No frameworks, npm packages or build tools are required.

## Features
- Start, pause, resume and reset
- Hours, minutes, seconds and centiseconds
- Lap duration and cumulative time
- Fastest and slowest lap indicators
- Export lap history to CSV
- Light/dark theme saved in Local Storage
- Optional button sound using the Web Audio API
- Keyboard shortcuts: Space (start/pause), L (lap), R (reset while paused)
- Responsive mobile, tablet and desktop layout
- Accurate elapsed-time calculation using `performance.now()`

## Folder structure
```text
project-05-stopwatch/
├── index.html
├── css/style.css
├── js/app.js
└── README.md
```

## Run locally
Extract the ZIP, open the folder in VS Code and run `index.html` with Live Server, or open it directly in your browser. No install/build step is needed.

## Deploy
**GitHub Pages:** Push the extracted project files to a GitHub repository. Go to Settings → Pages → Deploy from a branch, select `main` and `/(root)`.

**Vercel:** Import the GitHub repository, select Other as the framework preset, leave the build command empty, set output directory to `.`, then deploy.

## Main JavaScript functions
- `toggle()` — starts, pauses or resumes the stopwatch.
- `reset()` — resets elapsed time and lap records.
- `recordLap()` — records lap and cumulative time.
- `display()` — updates the time display.
- `renderLaps()` — renders lap records and fastest/slowest labels.
- `exportCSV()` — downloads lap records as CSV.

Lap history is kept for the current browser session and can be exported as a CSV file.
