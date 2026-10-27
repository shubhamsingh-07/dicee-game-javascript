# Dicee — Dice Game

[![Language](https://img.shields.io/badge/HTML-CSS-JavaScript-blue.svg)](https://developer.mozilla.org/)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)

A small browser-based dice game built with HTML, CSS, and vanilla JavaScript. Reload the page to roll two virtual dice and see whether Player 1 wins, Player 2 wins, or the result is a draw.

## Features

- Generates a random result from 1 to 6 for each player on page load.
- Updates each player's dice image to match the generated result.
- Displays the winner or a draw in the page heading.
- Uses six local PNG images for the dice faces.
- Includes a simple, styled layout with Google Fonts.

## Built With

- **HTML5** for page structure
- **CSS3** for styling and layout
- **JavaScript** for random dice rolls and winner selection
- **Google Fonts** for the Lobster and Indie Flower typefaces

## Project Structure

```text
dicee-game-javascript/
├── dicee.html
├── styles.css
├── index.js
└── images/
    ├── dice1.png
    ├── dice2.png
    ├── dice3.png
    ├── dice4.png
    ├── dice5.png
    └── dice6.png
```

## Run Locally

No build tools, package installation, or server-side code are required.

1. Clone or download this repository.
2. Open `dicee.html` in a modern web browser.
3. Refresh the page to roll the dice again.

The page loads `index.js`, which generates two random values, updates the dice images, and changes the heading to show the result.

## How the Game Works

1. JavaScript generates one random integer from 1 to 6 for each player.
2. Each number selects the corresponding image in the `images/` directory.
3. The two values are compared:
   - Equal values display **DRAW!!**
   - A higher Player 1 value displays **PLAYER 1 WINS!!**
   - Otherwise, **PLAYER 2 WINS!!** is displayed.

This is a single-page, single-round game. The result is recalculated when the page is reloaded; there is no score tracking or in-page roll button in the current version.

## Learning Outcomes

This project is useful for practicing:

- Generating random integers with `Math.random()` and `Math.floor()`
- Selecting and updating DOM elements
- Changing image attributes dynamically
- Comparing values with conditional statements
- Organizing a small front-end project into HTML, CSS, JavaScript, and image assets

## Known Improvements

- `dicee.html` currently contains a stylesheet link pointing to `index.js`. JavaScript is already included correctly with a script element, so the incorrect stylesheet link can be removed.
- Add responsive layout rules for smaller screens.
- Add a **Roll Again** button so users do not need to reload the page.
- Add score tracking across multiple rounds.
- Add alternative text to the dice images for better accessibility.

These are documentation notes; this README update does not change the application code.

## Asset and Font Notes

The six dice images are stored locally, while the fonts are loaded from Google Fonts. The repository does not document the original source or licensing terms for the image assets. Confirm that you have redistribution rights for all third-party assets before publishing or reusing them. The MIT License for this repository does not override any separate third-party asset or font terms.

## License

The project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
