# Hangman

This app will serve to practice more game logic, as well as implement the principles discussed in the previous few apps like coinflip and state design.

Colt provided starter code for this example and I will be modifying that solution.

## Requirements

* Add keys. Buttons current do not have unique key prop.

* Number of Wrong Guesses. Add some detailing text about how many wrong guesses have been made.

* End Game on Loss

Game only starts with 6 guesses by default, so it should only allow 6 wrong guesses. Right now it doesn't stop the game and allows continued guessing which ends up breaking the images. (Use a property for maxGuesses so the game can be dynamic)

* Alt Text. Add alts to the image that explains the gamestate for accessibility.

* Random Word. By default the word is always apply. Data provided in words.js list of words and a function returning a random word. Incorporate this so the game uses this to choose a secret word.

* Add Restart button. Button that restarts the game. Should pick a new random word and reset list of guessed letters and number of wrong guesses.
