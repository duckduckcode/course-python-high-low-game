# Concepts

Goal: Briefly experiment with each of the concepts covered by this activity

## Printing plain text

```
print("Hello! This is some text.")
```

❯ Hello, this is some text.

## Printing plain text, plus a string variable

```
name = "Mickey"
print("Hello! My name is " + name)
```

❯ Hello! My name is Mickey

## Printing plain text, plus a numeric variable

```
number = 42
print("The meaning of life is " + str(number))
```

❯ The meaning of life is 42

## Capturing text input

```
name = input("Please enter your name: ")
print("Your name is " + name)
```

❯ Please enter your name:  Mickey
❯ Your name is Mickey

## Capturing numeric input (whole numbers)

```
age_str = input("Please enter your age:")
print("Your age is " + age_str)

age_int = int(age)
age_in_five_years = age_int + 5
print("In 5 years you will be " + str(age_in_five_years))
```

❯ Please enter your age: 15
❯ Your age is 15
❯ In 5 years you will be 20

## Random integer (whole number)

```
import random

number = random.randint(1, 100)
print("This number is between 1 and 100: " + str(number))
```

❯ This number is between 1 and 100: 32

## Single condition

```
password = "Password123"
user_input = input("Please enter the password: ")

if user_input == password:
  print("Password is correct")
```

❯ Please enter the password: Password123
❯ Password is correct

## Single condition with "else"

```
password = "Password123"
user_input = input("Please enter the password: ")

if user_input == password:
  print("Password is correct")
else:
  print("Sorry, that password is incorrect")
```

❯ Please enter the password: password12
❯ Sorry, that password is incorrect
❯ Please enter the password: Password123
❯ Password is correct

## Multiple conditions

```
player_score = 1500

if player_score > 1000:
    print("Player achieved GOLD")
elif player_score > 800:
    print("Player achieved SILVER")
elif player_score > 600:
    print("Player achieved BRONZE")
    
print("Game over")
```

❯ player_score = 1500
❯ Player achieved GOLD
❯ Game over
❯ player_score = 850
❯ Player achieved SILVER
❯ Game over
❯ player_score = 650
❯ Player achieved BRONZE
❯ Game over
❯ player_score = 600
❯ Game over

## Repeat a set number of times

```
for number in range(3):
    print("repeat #" + str(number))
```

❯ Repeat #0
❯ Repeat #1
❯ Repeat #2

## Repeat as long as a condition is true

```
keep_repeating = True

while keep_repeating == True:
    user_input = input("Please enter the letter A: ")
    
    if user_input == "A":
        print("Thank you!")
        keep_repeating = False
```

❯ Please enter the letter A: A
❯ Thank you!
❯ Please enter the letter A: b
❯ Please enter the letter A: a
❯ Please enter the letter A: A
❯ Thank you!

## Capturing errors

```
user_input = input("Please enter an integer:")

try:
    number = int(user_input)
    print("Thank you!")
except:
    print("Sorry that is not a valid integer")
```

❯ Please enter an integer: 100
❯ Thank you!
❯ Please enter an integer: hello
❯ Sorry that is not a valid integer