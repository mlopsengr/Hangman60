# Hangman60
This project builds a game, leveraging on effective use of classes and functions, that prompts a player to
guess the letters in a random word. If all the letters within the word is guessed correctly within the
chances available, the player wins.

## Milestone 1
- This milestone aimed to ask a player for an input, ultimately, a letter. It builds object oriented structure around each function intended to support checking if a letter has been used, if the letter is in the guessed word and the number of lives left.

- Within this function, a while statement is used to ensure that a letter is not inputed more than once by the player by checking a list that stores the inputs
```python
while self.letter in self.list_letters:
            self.letter = input("You have already tried this letter. Please enter a letter: ")
```
- The function also ensures only one letter is inputed at a time using a conditional statement
```python
  while len(self.letter) != 1:
            self.letter = input("Please enter a single letter: ")
```

## Milestone 2
- This is where the variables to be used where initialised. These variables include the list of words, encoded as 'word_list' and the initial number of lives as 'num_lives'.
- This milsestone essentially is the foundation of the object oriented programming (OOP) structure on which the game is built

## Milestone 3
- The 'ask_letter' method of the game class is built, which prompts the user for a letter input
```python
self.letter = input("Please enter a letter: ")
```
- Within this function, the while statement is used to ensure that a letter is not tried more than once, by checking a varaible 'list_letters', a list of letters inputed by the player. It also uses a conditional statement to ensure multiple letters are not entered at a time.

## Milestone 4
- This focuses on the logic of the game,where the user is prompted to keep inputting a letter until the user guesses the word right.
- If the word is not guuessed right within the number of lives available, the game ends and the user his told he lost.
```python
while game.num_lives > 0 and '_' in game.word_guessed:
        game.ask_letter()
        print(game.word_guessed)
    if game.num_lives > 0:
        print("Congratulations, you won!") # message on winning
    else:
        print("You ran out of lives, The word was:", game.word)
```


