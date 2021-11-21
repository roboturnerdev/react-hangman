# Hangman

This app will serve to practice more game logic, as well as implement the principles discussed in the previous few apps like coinflip and state design.

Colt provided starter code for this example and I will be modifying that solution.

## Complete: Takeaways

### Lots of Game Logic

* Multiple phases of creating this simple hangman game. First had simple logic showing buttons and whether or not you've lost. Eventually changed it up to create isWinner and gameOver to determine 'gameState' separate from 'this.state'.

* Would refactor gameState into its own method if I did any more than what's in the solution.

### Use of Set, Array.split, Array.join, Array.map

* These array functions are critical to React so far. Getting good practice in with Sets or mapping over arrays and performing callbacks on the items is a common pattern.

<img src="https://i.imgur.com/aOO4fyT.png">
<img src="https://i.imgur.com/jcrpBwf.png">
<img src="https://i.imgur.com/yD5D3Pi.png">
<img src="https://i.imgur.com/9J99xXK.png">

# Original Post

## Requirements

* Add keys. Buttons current do not have unique key prop.

* Number of Wrong Guesses. Add some detailing text about how many wrong guesses have been made.

* End Game on Loss

Game only starts with 6 guesses by default, so it should only allow 6 wrong guesses. Right now it doesn't stop the game and allows continued guessing which ends up breaking the images. (Use a property for maxGuesses so the game can be dynamic)

* Alt Text. Add alts to the image that explains the gamestate for accessibility.

* Random Word. By default the word is always apple. Data provided in words.js list of words and a function returning a random word. Incorporate this so the game uses this to choose a secret word.

* Add Restart button. Button that restarts the game. Should pick a new random word and reset list of guessed letters and number of wrong guesses.
