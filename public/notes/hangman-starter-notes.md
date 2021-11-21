# hangman starter code notes

I am going to document what I read from opening the inital project and take notes. This way, I can plan my state design and also game logic based on how the app is already constructed.

## Index.js and App.js

Index draws an App, App draws a Hangman. Pretty straight forward doesn't pass anything in at the moment to Hangman.

## Hangman.js

Default Props:
  - maxWrong 6		// here its 6 but will be changed to be dynamic
  - images[] 		// array of the imported images

constructor:
  - super props
  - initial state: 
    - nWrong: 0			// wrong guesses
    - guessed: new Set()	// i am thinking this is the characters guessed incorrectly
    - answer: "apple"		// the solution to the game word
  - bind the handleGuess function to *this*

### methods

* guessedWord - this method shows the curent-state of the word, if guessed letters are a, p, e show app_e for "apple"
  - this function operates by setting the state of answer to the result of a chained .split .map on the guessed Set.

* handleGuess(e) - handle a guessed letter. 1. add to guessed letters, 2. if not in answer, add to number wrong
  - sets state of guessed by adding letter to it and sets state of nWrong to add one if answer does not include the letter.

* generateButtons - returns array of letter buttons. maps over the string abc..z and each letter creates a button for it with handleGuess onclick

* render
  - h1 title
  - image where the src is {this.props.images[this.state.nWrong]} // this should make it draw the correct state of hangman based on how many incorrect guesses
  - p of guessedWord
  - p of generateButtons (draws the letters you can select)


