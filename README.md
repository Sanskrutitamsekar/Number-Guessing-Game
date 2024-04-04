# Number-Guessing-Game
import random

def number_guessing_game():
    print("Hello and Welcome to the Number Guessing Game!")
    print("I have selected a random number between 1 and 100. Try to guess it!")

    # Generate a random number between 1 and 100
    secret_number = random.randint(1, 100)

    # Initialize the number of guesses
    num_guesses = 0

    while True:
        guess = int(input("Please guess the number (between 1 and 100): "))
        num_guesses += 1

        # To check if the guessed number is correct
        if guess == secret_number:
            print(f"Yayyy! You guessed the correct number {secret_number} in {num_guesses} guesses.")
            break
        elif guess < secret_number:
            print("Oops the number too low! Try a higher number.")
        else:
            print("Oops the number too high! Try a lower number.")

# Start the game
number_guessing_game()


