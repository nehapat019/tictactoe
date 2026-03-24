# CLAUDE.md

This file provides guidance to Claude Code (claude.ai/code) when working with code in this repository.

## Overview

This directory currently contains a single-file web game (`tictactoe.html`) — a self-contained HTML/CSS/JavaScript Tic Tac Toe game with no build system or dependencies.

## Running the Project

Open `tictactoe.html` directly in any browser:

```bash
open tictactoe.html
```

## Architecture

`tictactoe.html` is a single file containing all HTML, CSS, and JavaScript inline:

- **Board state** — a flat 9-element array (`board[]`) representing the grid
- **Game logic** — `checkWinner()` tests all 8 win conditions; `endGame()` handles scoring and highlighting
- **AI (vs Computer mode)** — unbeatable minimax algorithm in `minimax()` / `computerMove()`
- **Scoring** — tracked in a `scores` object (`X`, `O`, `D`) and updated in the DOM after each game
