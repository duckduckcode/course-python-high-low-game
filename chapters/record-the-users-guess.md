# Record the user's guess

Goal: Capture the user's guess so later we can test if it's correct

## Steps to record the user's guess

- Write a comment explaining the purpose of the code
- Use the input function to wait for user input
- Use a variable to store the user's guess for later use

**Reading Example Code**
Remember that **black code** you already have,
and **coloured code** you need to add.

```
print("High Low Game")

# tell the user the range of numbers to guess from
print("I'm thinking of a number between 1 and 100")
```

```
# prompt the user to guess a number, and save the value
user_guess = input("Guess a number and press enter: ")
```

**Run your code**
You should see the message "Guess a number..."
The script should wait for a number to be entered.

## Steps to confirm the user's guess

- Write a **comment** explaining the purpose of the code
- Use the **print function** to display a message plus the user's guess.

```
print("High Low Game")

# tell the user the range of numbers to guess from
print("I'm thinking of a number between 1 and 100")

# prompt the user to guess a number, and save the value
user_guess = input("Guess a number and press enter: ")
```

```
# tell the user the number they guessed
print("You guessed the number " + user_guess)
```

**Run your code**
After a number is entered, you should see "You guessed..."
