import random

print("Guessing Game")

number = random.randint(1, 10)
guess = None
count = 0

while guess != number:
    guess = int(input("Guess a number between 1 and 10: "))
    count += 1
    if guess < number:
        print("Too low!")
    elif guess > number:
        print("Too high!")
    else:
        print("Congratulations, you guessed the number!")
        print("It took you", count, "tries.")
