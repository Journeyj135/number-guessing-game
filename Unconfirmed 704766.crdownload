# A simple Number Guessing Game
print("\n________________THE GUESSING GAME_________________\n")
print("""This is a guessing game that ranges from 1 - 100
you have seven (7) tries to guess the correct number
do you have skills required to win? Lets Play!\n""")

import random

# Correct number to guess
random_number = random.randint(0, 100)

# How many chances player has
chances = 7
count = 7

# Number of chances taken
guesses = 0

# Ask user for a number
while guesses < chances:
    guesses += 1

    try:
        guess = int(input("Guess the Number: "))

    except ValueError:
        print("Please insert a number between 1 - 100.")
        continue

    if guesses == 7:
        print(f"-------------Game Over!---------------\n    You have used all your guesses: {chances} / 7")
        print(f"    Correct Answer: {random_number}")
        break

    if guess == random_number:
        print(
            f"--------Congradulations!------------\n  The Correct answer was {random_number}\n    Guesses Taken: {guesses} out of 7")
        break

    elif guess > random_number:
        count -= 1
        print(f"{guess} is too high\nChances Left: {count}")

    elif guess < random_number:
        count -= 1
        print(f"{guess} is too low\nChances Left: {count}")
