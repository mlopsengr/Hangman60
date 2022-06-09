# Hangman60
This project builds a game, leveraging on effective use of classes and functions, that prompts a player to
guess the letters in a random word. There is limited amount of chances implemented as the "players number of lives"
and with each failed attempt, its value reduces. If all the letters within the word is guessed correctly within the
chances available, the player wins.

## Milestone 1
- This milestone aimed to ask a player for an input, ultimately, a letter
- A function,'ask_letter", is implemented to prompt the user for an input
'''python
self.letter = input("Please enter a letter: ")
'''
- Within this function, a while statement is used to ensure that a letter is not inputed more than once by the player by checking a list that stores the inputs
'''python
while self.letter in self.list_letters:
            self.letter = input("You have already tried this letter. Please enter a letter: ")
'''
- The function also ensures only one letter is inputed at a time using a conditional statement
'''python
  while len(self.letter) != 1:
            self.letter = input("Please enter a single letter: ")
'''

## Milestone 2

