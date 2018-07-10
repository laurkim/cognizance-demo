# Cognizance

## Description
This is a demo for Cognizance, a cognitive learning memory game built in JavaScript with a Ruby on Rails backend. The purpose of the game is to find the pairs for all cards that match as quickly as possible, with as few clicks as possible.

## Core Features
1. [Immediate Validation on Card Flip](#immediate-validation-on-card-flip)
2. [Increasing Levels of Difficulty](#increasing-levels-of-difficulty)
3. [User Account Creation](#user-account-creation)






![Cognizance Game Over](demo-gifs/game-over.gif)

![Cognizance Game Restart](demo-gifs/game-restart.gif)

### Immediate Validation on Card Flip
When a user chooses a difficulty and starts the game, there is a countdown during which all functionality for the board where the cards are rendered is disabled. Once the game begins, a timer starts to keep track of the duration of the game. A user can click on a card in intervals of two at a time.

The game logic accounts for matches in images by leaving them flipped with the image displayed for the remaining portion of the game and making both cards static with all click actions for those specific cards disabled. If the card images do not match, they are flipped back to the back face of the card and will continue to have the functionality to click and flip them until the match is found and the action disabled.

![Cognizance Pairs Matched](demo-gifs/game-matches.gif)

### Increasing Levels of Difficulty
There are four levels of difficulty:
  - Basic: One row of cards is rendered for understanding how the game should function in its most simplest form
  - Easy: Two rows of cards are rendered for initial skill-building once a user gets comfortable with the basic version
  - Medium: Three rows of cards are rendered for intermediate skill-building once a user is able to complete the Easy level with minimal amount of clicks
  - Hard: Four rows of cards are rendered for advanced skill-building once a user is able to complete the Medium level with the fewest clicks possible

![Cognizance Difficulty](demo-gifs/game-difficulty.gif)

### User Account Creation
The game will account for whether or not a user is logged in. When there is no one logged in, it will display a message.

![Cognizance Login](demo-gifs/game-login.gif)
