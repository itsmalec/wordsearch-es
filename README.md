# Sopa de Letras 🔎

A single-player Spanish word search toy. Pick a themed category, drag or tap to find the 8 hidden words, and learn each one's definition as you go.

## Play

Just open `index.html` in a browser — no build step, no dependencies.

## Categories

Animales, Colores, Comida, Familia, Países, Capitales. The last two are linked: each country's definition names its capital, and vice versa.

## Features

- 12×12 letter grid, randomized fresh every play (horizontal, vertical, and diagonal placements, forward-reading only)
- Definitions revealed the moment a word is found
- Best time per category, saved locally in the browser
- An automatic hint after 5 minutes of no progress
- Mouse-drag and touch-drag selection

## Project structure

The game itself lives in one file, `index.html` (inline CSS and JS), by design — see [CONTEXT.md](./CONTEXT.md) for the domain vocabulary used throughout. `www/index.html` is a copy of that file (Capacitor's required web asset folder) kept in sync by `npm run copy-www`; always edit the root `index.html`, never `www/index.html` directly.

## Android build (via Capacitor)

Requires Node.js, plus Android Studio / the Android SDK, on your own machine — this isn't built from inside the chat session.

```bash
npm install
npx cap add android   # one-time: generates the native android/ project
npm run android        # copies the latest index.html into www/, syncs, then opens Android Studio
```

Just re-run `npm run android` (or `npm run sync`) after any change to `index.html` — both always copy the latest version into `www/` first, so the app in Android Studio never goes stale.
