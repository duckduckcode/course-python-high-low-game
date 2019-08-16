# Generate a secret number

Goal: Generate a secret number for the user to guess

## Steps to generate a random number

- **Import** the python package called "random"
- Write a **comment** explaining the purpose of the code
- Use the **random.randint function** to generate the random number
- Pass the randint function two **parameters**
  - the minimum number
  - the maximum number
- Use a **variable** to save the random number for later use

::: callout-info
**Two new code blocks!**
Make sure you add both new code blocks. One to import the "random" package, and the other to generate the secret number.
:::

```
import random
```

```
print("High Low Game")
```

```
# generate a random number between 1 and 100
secret_number = random.randint(1, 100)
```

```
# tell the user the range of numbers to guess from
print("I'm thinking of a number between 1 and 100")

# prompt the user to guess a number, and save the value
user_guess = input("Guess a number and press enter: ")

# tell the user the number they guessed
print("You guessed the number " + user_guess)
```

::: callout-checkpoint
**Run your code**
Nothing will change about how the program runs.
It should run without errors.
:::

## Help! Errors!

::: callout-error
```
Traceback (most recent call last):
  File "python", line 3, in <module>
NameError: name 'random' is not defined
```
:::

**NameError: name 'random' is not defined**
This error says "random" is not a thing that exists in the script. This could be caused by:

- You did not add the code to `import random` at the top of your script.
- You spelled "random" incorrectly in the line `import random` at the top of your script.
