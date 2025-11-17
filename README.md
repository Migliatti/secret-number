# Secret Number Game

## Overview

Small browser game built during the Alura learning path to practice Git/GitHub workflows while reinforcing core JavaScript concepts. The interface invites the player to guess a random number between 1 and 10, and every hint is read aloud via the ResponsiveVoice API, making the experience playful and accessible.

## Features

- Random secret number that never repeats until the full range is exhausted
- Voice feedback (Brazilian Portuguese) for every prompt and hint
- Attempt counter with singular/plural handling in the success message
- New-game flow that re-enables once the secret is discovered
- Responsive layout with Chakra Petch + Inter typography

## Tech Stack

- HTML5 + CSS3 for the layout and styling
- Vanilla JavaScript for the game logic (`app.js`)
- ResponsiveVoice CDN for text-to-speech feedback

## Getting Started

```bash
git clone https://github.com/<your-username>/secret-number.git
cd secret-number
```

Open `index.html` directly in your browser or use any static server (e.g., VS Code Live Server). No build step is required.

## How to Play

1. Pick a number between 1 and 10 and enter it in the input box.
2. Click `Chutar` (Guess) to submit.
3. Follow the spoken hints—“maior” or “menor”—until you hit the secret number.
4. When you win, review how many attempts it took and click `Novo jogo` to restart.

## Project Structure

- `index.html` — base markup and component wiring
- `style.css` — visual theme, gradients, and responsive tweaks
- `app.js` — core logic: random number generation, attempts, TTS integration
- `img/` — illustration and background textures

## Next Steps

- Add difficulty levels by expanding `numeroLimite`
- Persist best scores using `localStorage`
- Translate UI strings for bilingual play

## License

This project is shared for learning purposes. Feel free to fork it, explore new ideas, and credit the original Alura coursework when appropriate.
