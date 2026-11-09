# Pote Gear Viewer: releases

Installers and automatic app updates for **Pote Gear Viewer**, a Windows 3D viewer for designing weapon and armour sets for Warhallow (PotE).

Download `PoteGearViewer-win-Setup.exe` from the latest release. Once it's installed, the app updates itself from this repository.

## What is (and isn't) here

- **Here:** the viewer application only, as an installer, a portable zip and Velopack update packages.
- **Not here:** no game files, models, textures or game data. On first run the viewer reads models from **your own installed game client**, without modifying it, and builds its data on your PC.
- **Game-data pack:** the viewer also needs a small game-data pack, which is distributed separately through a private repository. Ask the project owner for access and a read-only GitHub token, then add it in the app (Pote menu > Set GitHub token).

## Notes

- The builds are **unsigned**, so Windows SmartScreen may warn on first run ("More info" > "Run anyway").
- The viewer only reads the game client. It never runs, patches or injects into the game.
- The Oodle decompression library is not bundled. The app asks for your consent before fetching it on your PC.
