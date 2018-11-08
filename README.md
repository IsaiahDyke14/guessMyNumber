# guessMyNumber
import random

secret = random.randint(1,99) # Generate random integers between 1 and 99

guess = 0
tries = 0
print("Can you guess my number")
print("My number is a integer between 1 anad 99")

while guess != secret and tries < 6 :
    print ("whats your guess")
    guess = int(input())
    if guess < secret :
        print("Too low")
    elif guess > secret:
        print("Too High")

    tries = tries + 1

    if guess == secret :
        print(" You got it!")
    else :
        print("Nope! Try again, trash")
print("The secret number is secret = ", secret)
