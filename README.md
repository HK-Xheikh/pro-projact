# Guess the Number Game

# Set the secret number
secret_number = 42

# Initialize the number of attempts
attempts = 0

# Game loop
while True:
  # Ask the user to guess the number
  user_guess = int(input("Guess a number between 1 and 100: "))

  # Increment the number of attempts
  attempts += 1

  # Check if the user guessed correctly
  if user_guess == secret_number:
    print(f" Congratulations! You guessed the number in {attempts} attempts.")
    break

  # Check if the user's guess is too high or too low
  elif user_guess > secret_number:
    print("Your guess is too high. Try again!")
  else:
    print("Your guess is too low. Try again!")
