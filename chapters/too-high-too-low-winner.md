# Too high, too low, winner!

Goal: Provide feedback to the user that they guessed too low, too high, or just right

## Steps to tell the player too low, too high, winner!

- Add a condition to check if the number is too high
- Use the print function to say the number is too high
- Add a condition to check if the number is too low
- Use the print function to say the number is too low
- Add a condition to check if the number is exactly correct
- Use the print function to say the player won the game

```
import random

print("High Low Game")

# generate a random number between 1 and 100
secret_number = random.randint(1, 100)

# tell the user the range of numbers to guess from
print("I'm thinking of a number between 1 and 100")

# prompt the user to guess a number, and save the value
user_guess = input("Guess a number and press enter: ")

# tell the user the number they guessed
print("You guessed the number " + user_guess)
```

```
# check if the number is too high
if user_guess > secret_number:
  print("Too high, guess again")
  
# check if the number is too low
elif user_guess < secret_number:
  print("Too low, guess again")
  
# check if the number is correct
elif user_guess == secret_number:
  print("Hooray! You won!")
```

**Run your code**
You should get an error! Find out how to fix the error below.

## Help! Errors!
```
Traceback (most recent call last):
  File "python", line 16, in <module>
TypeError: '>' not supported between instances of 'str' and 'int'
```

**TypeError: '>' not supported between instances of 'str' and 'int'**
You can only use "greater than" or "less than" to compare two numbers. Our secret_number is a number, and our user_guess is a number... except that it's not!

The user_guess is actually a string!

When you use the input function to capture user input, the result is always a string. That is because Python doesn't know if the user entered a number - they might have typed in a word.

In Python, these two values are different - one is a string, one is an integer:

```
number_as_string = "42"
number_as_integer = 42
```

By default, the input function gives us a number formatted like the first example. To compare it with our secret number, it needs to be formatted like the second example.

It's up to us to tell Python to treat the user's guess as a number.

## Steps to change the user_guess input to a number
**
- Use a new **variable** to store the user_guess as a number
- Use the **int function** to change the user_guess to a number
- Compare the secret_number with the new user_guess_number in each **condition**

```
import random

print("High Low Game")

# generate a random number between 1 and 100
secret_number = random.randint(1, 101)

# tell the user the range of numbers to guess from
print("I'm thinking of a number between 1 and 100")

# prompt the user to guess a number, and save the value
user_guess = input("Guess a number and press enter: ")

# tell the user the number they guessed
print("You guessed the number " + user_guess)
```

```
# change the user guess from a string to a number
# so that we can compare it with the secret number
user_guess_number = int(user_guess)
```

```
# check if the number is too high
if user_guess_number > secret_number:
  print("Too high, guess again")

# check if the number is too low
elif user_guess_number < secret_number:
  print("Too low, guess again")

# check if the number is correct
elif user_guess_number == secret_number:
  print("Hooray! You won!")
```

**Run your code**
You should see "Too high" or "Too low" or "You won" when you enter a number.
The script should stop running after you have entered just one guess.