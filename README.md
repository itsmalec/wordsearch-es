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

Everything lives in one file, `index.html` (inline CSS and JS), by design — see [CONTEXT.md](./CONTEXT.md) for the domain vocabulary used throughout.
