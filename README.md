# Emberwatch: The Shattered Pass — v0.12.1

A self-contained browser tower-defence prototype. This is an original project and does not include Kingdom Rush assets or branding.

## Run locally
1. Download and extract the ZIP.
2. Open `index.html` in a modern browser.
3. For best results, serve the folder with a local static server (for example, `python -m http.server 8000`) and visit `http://localhost:8000`.

## GitHub Pages
1. Create a GitHub repository.
2. Upload the contents of this folder (especially `index.html`) to the repository root.
3. In repository Settings → Pages, select deployment from the `main` branch and `/ (root)`.
4. Save; GitHub Pages will publish the game when the workflow completes.

## Current prototype features
- Three campaign locations, with later missions unlocked by completing the previous mission.
- Tower construction, upgrades, specialisation, and selling.
- Archer, Mage, Cannon, and Barracks tower types.
- Moving hero, hero skill, meteor spell, enemy waves, elites and bosses.
- Hero training using medals earned from mission victories.
- Browser-local progress storage using `localStorage`.

## Known prototype limitations
- Progress is stored locally in the current browser/device; it does not sync across devices.
- Art is drawn with Canvas shapes rather than production sprite sheets.
- Audio, cloud saves, multiplayer, and native iOS packaging are not included.
- This is a prototype, not an App Store release.

## Version
`0.12.1`


## v0.12.1 hotfix
- Fixed the canvas rendering context variable mismatch (`ctx` vs `g`) that stopped the animation loop on the first frame. The battlefield now renders continuously so wave spawns, enemy movement, tower attacks, and hero combat can update.
