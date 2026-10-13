# THE CITY HAS SECRETS — playable browser prototype

A small, playable Three.js first-person horror mystery prototype with a live field map, clue markers, journal, flashlight battery, atmospheric synthesized sound, and a first chapter objective chain.

## Run it
Because this uses JavaScript modules, run it from a local web server rather than opening `index.html` directly.

### Option A: VS Code
1. Put `index.html` in a folder.
2. Install the **Live Server** extension.
3. Right-click `index.html` → **Open with Live Server**.

### Option B: Python
From this folder run:
```bash
python -m http.server 8000
```
Then open `http://localhost:8000`.

## Deploy to GitHub Pages
1. Create or open your repository.
2. Upload `index.html` and `README.md` to the repository root.
3. In **Settings → Pages**, choose **Deploy from a branch**, select `main` and `/(root)`, then Save.
4. Wait for GitHub Pages to publish the site.

## Controls
- **WASD / arrows:** move
- **Mouse:** look around (click the scene to capture the mouse)
- **Shift:** run
- **C:** crouch
- **E:** investigate / collect clue
- **F:** flashlight on/off
- **J:** journal and full map
- **Esc:** pause
- Mobile: on-screen movement and investigate controls

## Map
The top-right field map shows your position in yellow and uncollected evidence/objectives in cyan/red. Press **J** to open the larger map and evidence journal. Follow the objective text at the upper left.

## Notes
- This is a starter chapter/prototype, not a finished AAA open-world game. It uses procedurally assembled geometry and synthesized audio so it can run without a large asset download.
- Three.js is loaded from jsDelivr, so an internet connection is needed.
- Browser audio starts after you begin the game due to browser autoplay restrictions.
- Use only audio/assets you have permission to distribute. For a production version, replace placeholder geometry with optimized licensed models, authored voice recordings, and tested collision/navigation systems.
