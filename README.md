# Emoji Game

## Overview

This project is a simple and interactive **Emoji Game** built with ReactJS. The objective of the game is to click on each emoji exactly once without clicking any emoji more than once. The game keeps track of your current score and top score, providing an engaging experience as you try to beat your previous best.

## Features

- **Initial State**: The game starts with both the score and the top score set to 0.
- **Game Play**:
  - Clicking on an emoji that hasn't been clicked before increments the score by one.
  - Clicking on an already clicked emoji ends the game.
  - Clicking all emojis exactly once wins the game.
  - The top score is updated if the current score exceeds the previous top score.
- **Game End**:
  - A "Won Game" view is displayed if all emojis are clicked once.
  - A "Lose Game" view is displayed if an emoji is clicked more than once.
- **Play Again**: The game can be restarted by clicking the "Play Again" button, which resets the current score but retains the top score.

## Component Structure

### Main Components

- **EmojiGame**: The main component that holds the state and logic for the game.
- **NavBar**: Displays the game logo, current score, and top score.
- **EmojiCard**: Represents each emoji card in the game.
- **WinOrLoseCard**: Displays the result (win or lose) and provides the option to play again.

### Component Breakdown

- **EmojiGame**
  - Receives `emojisList` prop containing emoji objects.
  - Manages game state including the list of clicked emojis, current score, and top score.
  - Handles game logic such as updating the score and determining win/loss conditions.
- **NavBar**
  - Displays the logo, current score, and top score.
- **EmojiCard**
  - Displays an individual emoji.
  - Handles click events to update the game state.
- **WinOrLoseCard**
  - Displays the win or lose message and image.
  - Provides the "Play Again" button to restart the game.

## Design Files

### Responsive Design

- **Small Screens**: ![Design for small screens](https://assets.ccbp.in/frontend/content/react-js/emoji-game-sm-outputs.png)
- **Large Screens**: 
  - ![Game View](https://assets.ccbp.in/frontend/content/react-js/emoji-game-lg-output-v2.png)
  - ![Won Game](https://assets.ccbp.in/frontend/content/react-js/emoji-game-won-game-lg-output.png)
  - ![Lose Game](https://assets.ccbp.in/frontend/content/react-js/emoji-game-lose-game-lg-output.png)

## Setup Instructions

1. **Install Dependencies**: Run `npm install` to install all necessary packages.
2. **Start the Application**: Run `npm start` to start the development server and launch the app in your default web browser.

## Quick Tips

- Use `cursor: pointer;` to change the cursor style when hovering over clickable elements.
- Use `outline: none;` to remove the outline when buttons and input elements are clicked.

## Colors and Fonts

### Colors

- **Primary Color**: #6a59ff
- **Text Colors**: #ffffff, #3d3d3d
- **Background Colors**: #9796f0, #fbc7d4, #ffffff33, #ffce27
- **Border Colors**: #ffffff30

### Font

- **Roboto**

## Image Resources

- **Emoji Logo**: ![Emoji Logo](https://assets.ccbp.in/frontend/react-js/game-logo-img.png)
- **Won Game Image**: ![Won Game](https://assets.ccbp.in/frontend/react-js/won-game-img.png)
- **Lose Game Image**: ![Lose Game](https://assets.ccbp.in/frontend/react-js/lose-game-img.png)

## Implementation Files

- **EmojiGame**: `src/components/EmojiGame/index.js`, `src/components/EmojiGame/index.css`
- **NavBar**: `src/components/NavBar/index.js`, `src/components/NavBar/index.css`
- **EmojiCard**: `src/components/EmojiCard/index.js`, `src/components/EmojiCard/index.css`
- **WinOrLoseCard**: `src/components/WinOrLoseCard/index.js`, `src/components/WinOrLoseCard/index.css`

## Important Notes

- Ensure all components are placed in the `src/components` directory.
- Do not change component folder names to pass tests.
- Emojis should have `alt` attributes with values from the `emojiName` key in each emoji object.

Enjoy playing the **Emoji Game** and aim for the highest score!
