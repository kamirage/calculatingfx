# Stop Loss Calculator — Electron build project

This repository contains an Electron wrapper around a local HTML Stop Loss calculator UI.

## How to build (automatic, using GitHub Actions)
1. Create a new GitHub repository and push these files to it (all files and folders from this archive).
2. Open the repository on GitHub and enable Actions (they are enabled by default).
3. The included GitHub Actions workflow (`.github/workflows/build.yml`) will run on push and produce a Windows build artifact (portable .zip/.exe).
4. After the workflow finishes, download the artifact from the Actions run — it contains the ready-to-run `.exe` and portable build.

## How to build locally (if you prefer)
- Requires Node.js and npm.
- Run:
  ```bash
  npm install
  npm run dist
  ```
- The final artifacts will be in the `dist/` folder.

## Notes
- This project uses `electron` + `electron-builder`.
- The HTML app lives in `app/stop_loss_calculator_with_max_loss.html`.
