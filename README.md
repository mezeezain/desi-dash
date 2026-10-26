# Desi Dash 🪁

A Mario-style 2D platformer starring Pakistani heroes, playable right in your browser on desktop and mobile.

A storm called **Andhi** has scattered the pieces of the giant festival kite across Pakistan. Pick your hero, run through Lahore, Karachi and the Thar desert, stomp Andhi's minions, collect jalebis and bring the colour back to the sky!

## ▶ Play

Once GitHub Pages is enabled, the game is live at:
`https://<your-username>.github.io/desi-dash/`

## Heroes

| Hero | From | Ability |
|------|------|---------|
| Ali | Lahore | Always throws cricket balls |
| Ayesha | Karachi | Fastest runner |
| Hamza | Peshawar | Starts every life big & strong |
| Zara | Hyderabad | Double jump |
| Bilal | Hunza | Wall slide & wall jump |
| Mahnoor | Islamabad | Hold jump to glide |

## Controls

| Action | Keyboard | Gamepad | Touch |
|--------|----------|---------|-------|
| Move | ← → / A D | D-pad / left stick | ◀ ▶ buttons |
| Jump (hold = higher) | Space / ↑ / W | A | A button |
| Run / throw ball | Shift (run), J (run + throw) | X | B button |
| Pause | Esc / P | — | II button |
| Mute (menu) | M | — | Sound toggle |

## Items

- **Jalebi**: coin, 100 = extra life
- **Taara (star)**: 3 hidden per level, 1000 points each
- **Matka block**: hit it from below for a power-up
  - **Samosa**: grow big (take one extra hit)
  - **Chai**: 1.5× speed for 10 s
  - **Patang**: glide for 10 s
  - **Cricket ball**: throw balls at enemies with J

## Run locally

No build step needed. Just serve the folder:

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

Add `?debug` to the URL to see physics hitboxes, or `?touch` to force the on-screen controls.

## Tech

- [Phaser 3.70](https://phaser.io) (bundled in `lib/` so the game works without a CDN)
- All art and sound is generated in code: no external assets
  - Outlined, shaded pixel-art heroes in shalwar kameez, dupattas, a pakol and a cricket kit
  - Three themed worlds: Lahore's havelis and Minar-e-Pakistan, Karachi's Clifton beach and
    Mazar-e-Quaid, and the Thar desert with Mohenjo-daro style ruins
  - Parallax backgrounds, a waving Pakistan flag at each finish, dust, sparkle and confetti effects
- Progress is saved in the browser's `localStorage`

## Credits & licence

Code released under the MIT licence. Phaser is © Phaser Studio, MIT licence.
Desi Dash is an original game inspired by classic platformers; it uses no Nintendo characters, art or audio.
