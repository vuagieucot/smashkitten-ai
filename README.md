# SmashKitten

A cartoon cat badminton game that runs in the browser. Play against the CPU or with a friend on one keyboard, or use touch controls on a phone.

> **Made by AI.** The game was built by an AI (Claude, by Anthropic) from the provided UI and character asset packs.

## Play

- Open `index.html` in a browser, or visit the hosted link.
- Modes: VS CPU (Easy, Normal, Hard) and 2 players on one keyboard.
- Four cats (Momo, Kai, Luna, Rocky), each with a special shot. Four courts.
- Rally-point scoring, win by 2. Match length: Quick, Standard or Classic.

## Controls

| Action  | Player 1 | Player 2 | Phone |
|---------|----------|----------|-------|
| Move    | A / D | ← / → | Stick |
| Jump    | W | ↑ | Flick stick up or JUMP |
| Dive    | S | ↓ | DIVE |
| Swing   | F or Space | `.` or Enter | SWING |
| Smash   | G | `/` | SMASH |
| Special | E | `;` | SPECIAL |

Hold toward the net while swinging for a drop shot. Esc pauses, M mutes. Gamepads work too.

## Phone and offline

- Touch controls turn on automatically on phones. The TOUCH CONTROLS button on the title screen toggles them.
- Once the game is hosted over https, it caches itself for offline play (`sw.js`). On iPhone: open the link in Safari, tap Share, then Add to Home Screen, and open it once while online.
- After changing any game files, bump `VERSION` in `sw.js` and update its file list so phones download the new version.

## Hosting (free)

Any static host works, for example GitHub Pages (Settings → Pages → Deploy from a branch → `main`, `/ (root)`) or Netlify Drop.

## Files

- `index.html`, `css/`, `js/`: the game (plain HTML, CSS and JavaScript, no build step)
- `assets/`: sprites cut from the asset packs
- `sw.js`, `manifest.webmanifest`, `icons/`: offline support and home-screen install
