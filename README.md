BRIEF

I wanted to do an extra game to concrete my knowledge.

In the game Hangman a random word is chosen by player 1 (computer).

On each turn the user guesses a letter. If the letter is in the word, it's revealed
If not points are deducted and a hangman image starts to appear.

User wins when they guess all letters of the word.
User loses when all points deducted / hangman appears fully.

APPROACH

1. In order to generate a random word/phrase I stored a list in an array.
2. On starting the game a word is chosen using Math.Random. The word is looped over and "\_" or "/" is generated. The game board is made visible using classList.remove.
3. User enters letter in an input box and clicks a button to submit their answer. This is converted to lowercase.
4. The app checks if the letter is included in the chosen word and updates a score accordingly
5. If so the letter replaces the relevant \_ in the hidden word.
   if not, part of the hangman appears (using classlist) which is based on the score

I found the main challenge seemed to be finding a way to show the user which letters they had already chosen. I started exploring an array, which had values pushed into it.
Then decided to display a complete alphabet and remove the letters from the alphabet array each turn, removing the ones the player has guessed.

checkScore is used to run gameOver if score is 0. If so a message will be revealed.

IMPROVEMENTS

Difficulty levels - could determine what level the score starts at.
