# Pote Gear Viewer: releases

Installers and automatic app updates for **Pote Gear Viewer**, a Windows 3D viewer for designing weapon and armour sets for Warhallow (PotE).

Download `PoteGearViewer-win-Setup.exe` from the latest release. Once it's installed, the app checks this repository for new versions. When one is available, it asks you before downloading it and restarting. Update checks don't need a GitHub token.

## What is (and isn't) here

- **Here:** the viewer application only, as an installer, a portable zip and Velopack update packages.
- **Not here:** no game files, models, textures or game data. On first run the viewer reads models from **your own installed game client**, without modifying it, and builds its data on your PC.
- **Game-data pack:** the viewer also needs a small game-data pack, kept in the private repository `Warhallow-Gear-Viewer/gear-viewer-data` for members of that organization:
  1. Ask the project owner to add you to the **Warhallow-Gear-Viewer** organization.
  2. On github.com, go to Settings > Developer settings > Personal access tokens > Fine-grained tokens > Generate new token.
  3. Set **Resource owner** to **Warhallow-Gear-Viewer**. Under **Repository access**, choose **Only select repositories** and pick **gear-viewer-data**. Under **Permissions**, set **Contents** to **Read-only**.
  4. Paste the token into the viewer's setup wizard when it asks. It's stored encrypted on your PC only. Never share it.

## Notes

- The builds are **unsigned**, so Windows SmartScreen may warn on first run ("More info" > "Run anyway").
- The viewer only reads the game client. It never runs, patches or injects into the game.
- The Oodle decompression library is not bundled. The app asks for your consent before fetching it on your PC.
