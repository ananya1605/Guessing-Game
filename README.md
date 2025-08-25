🎯 Number Guessing Game

A simple Python CLI game where the user has to guess a randomly generated number between 1 and 100.

## 🛠️ How to Run

1. Make sure Python is installed.
2. Run the script:

```bash
import random 
random.randint(1,100)
jackpot = random.randint(1,100)

guess = int(input('Guess the number : '))
counter = 1

while guess != jackpot:
    if guess < jackpot:
        print('Guess higher')
    else:
        print('Guess lower')
    guess = int(input('Guess again:'))
    counter += 1
    
print('Congrats, Right guess')
print("You took", counter , "attempts")
