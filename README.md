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

## Limitations

- Very large inputs can exceed JavaScript number precision or produce results that are too large to display reliably.
- The current UI is Spanish-only.
- Combination with repetition assumes the usual mathematical domain where `n` is positive.

## Possible Improvements

- Add a language toggle for Spanish and English.
- Add example problems for each operation type.
- Add automated tests for edge cases and large inputs.
- Deploy with GitHub Pages and link the live version from the repository description.

