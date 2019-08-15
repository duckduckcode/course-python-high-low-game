# Overview

The High-Low Game is a guessing game, where the player must try to guess the secret number.

## Essential Test Cases

1. When the script is run, the app says "I'm thinking of a number between 1 and 100."
2. The user is prompted with "Guess a number and press enter:"
3. When the number is too high, the game says "Nope, too high!"
4. When the number is too low, the game says "Sorry, too low!"
5. When the number is correct, the game says "Woohoo! You win!"
6. Each time the app is run, a different random number is used as the secret number.

## Secondary Test Cases
1. When the number is less than 1, the game says "The secret number is between 1 and 100."
2. When the number is greater than 100, the game says "The secret number is between 1 and 100."
3. When the value entered is not a valid number, the game says "That is not a valid number."

## Learning objectives

- **variables of at least two data types**
  - random number generated is an integer
  - user input is a string by default, must be cast to an integer
  - game state of finished / unfinished is a boolean
- **sequence (order-dependent code)**
  - welcome message must be displayed at the start of the game
  - user must be prompted for a guess before it can be checked
  - congratulations message shown at end of game
- **selection (conditional statements)**
  - if the number is higher, tell the user
  - if the number is lower, tell the user
  - if the number is the secret number, win the game
  - if the number is out of bounds, tell the user
  - if the guess is not a valid number, tell the user
- **iteration (loops)**
  - while the user hasn't guessed the number, the game continues
- **user input (or input from another source)**
  - the user must enter a number as their guess
- **handle expected values**
  - game responds to the user's guess so long as it is a number from 1 to 100
- **handle boundary values**
  - game responds to 1 as a valid guess, but 0 as an invalid guess
  - game responds to 100 as a valid guess, but 101 as an invalid guess
  - game responds to numbers greater than 100 as "too high"
  - game responds to numbers less than 1 as "too low"
- **handle invalid values**
  - game responds to non-numeric input with "input is not a number"
- **comments**
  - all logic should be explained by line or by section as appropriate
  - main logical areas of the code should be clearly labeled
- **~~constants~~**
  - not present in this learning exercise
- **~~derived values~~**
  - not present in this learning exercise
- **~~collections (lists or dictionaries)~~**
  - not present in this learning exercise
- **~~user-defined functions~~**
  - not present in this learning exercise