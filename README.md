# Number Guessing Game

## Overview
This is a simple Python-based number guessing game. The program generates a random number between 1 and 100, and the user must guess the number. The program provides feedback to guide the user toward the correct number and allows the user to quit at any time.

## Features
- Randomly generates a target number between 1 and 100.
- Provides hints to the user if their guess is too high or too low.
- Allows the user to quit the game at any time by entering 'Q'.
- Displays a success message when the user guesses the correct number.

## Prerequisites
To run this game, you need:
- **Python 3.x** installed on your system.

## How to Run
1. Copy the code below and save it in a `.py` file, for example, `number_guessing_game.py`:
   ```python
   import random

   target = random.randint(1, 100)

   while True:
       userChoice = input("guess the target or Quit(Q):")
       if userChoice == "Q":
           break

       userChoice = int(userChoice)
       if userChoice == target:
           print("success: correct guess!")
           break

       elif userChoice < target:
           print("your number was too small. take a bigger guess....")

       else:
           print("your number was too big. take a smaller guess....")

   print("-----------GAME OVER---------")
   ```

2. Open a terminal or command prompt.
3. Navigate to the directory where you saved the file.
4. Run the game using the command:
   ```bash
   python number_guessing_game.py
   ```

## Gameplay Instructions
1. The program will prompt you to guess the target number.
2. Enter your guess as an integer between 1 and 100.
3. The program will respond:
   - **Too small:** Your guess is smaller than the target number.
   - **Too big:** Your guess is larger than the target number.
   - **Correct guess:** You've guessed the target number and won the game.
4. To quit the game at any time, type `Q` and press Enter.
5. Once the game ends, a "GAME OVER" message is displayed.

## Example Output
```
guess the target or Quit(Q): 50
your number was too small. take a bigger guess....
guess the target or Quit(Q): 75
your number was too big. take a smaller guess....
guess the target or Quit(Q): 65
success: correct guess!
-----------GAME OVER---------
```

## Customization
- You can modify the range of the target number by changing this line in the code:
  ```python
  target = random.randint(1, 100)
  ```
  For example, to set the range to 1-50, replace it with:
  ```python
  target = random.randint(1, 50)
  ```

## License
This game is provided as open-source and can be freely modified or distributed.


