# Combinatoria

<p align="center">
  <img src="icono.png" alt="Combinatoria icon" width="96">
</p>

A lightweight browser-based calculator for common combinatorics operations. The app is designed as a quick educational tool for checking formulas such as permutations, variations, and combinations directly in the browser.

The interface is currently in Spanish.

## Features

- Calculates permutations using `n!`.
- Calculates variations without repetition using `n! / (n-r)!`.
- Calculates variations with repetition using `n^r`.
- Calculates combinations without repetition using `n! / (r! * (n-r)!)`.
- Calculates combinations with repetition using `(n+r-1)! / (r! * (n-1)!)`.
- Shows the formula used for each result.
- Runs entirely client-side with no dependencies, build step, or backend.

## Tech Stack

- HTML
- CSS
- JavaScript

## Running Locally

Clone the repository and open `index.html` in a browser:

```bash
git clone https://github.com/MarcosGibert/combinatoria.git
cd combinatoria
open index.html
```

You can also serve the folder locally if preferred:

```bash
python3 -m http.server 8000
```

Then visit `http://localhost:8000`.

## How It Works

Select the combinatorics operation, enter the required values for `n` and, when needed, `r`, and press **Calcular**. The app validates the most common invalid cases, performs the calculation in JavaScript, and displays both the result and the formula used.

## Project Context

This was built as a small personal learning project to make combinatorics formulas easier to experiment with. It focuses on a simple, accessible interaction model: choose an operation, enter values, and immediately see the result.

