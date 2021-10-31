# ⭐ Python Basics Cheat Sheet

## 🖨 Outputting information

```python
print("Hello, world!")       # Hello, world!
print("Hello, " + "world!")  # Hello, world!
```

## ❔ Asking for inputs

```python
name = input("Your name: ")  # User enters 'Bob'
print(name)                  # Bob
```

## 📜 Comments

```python
# This is a comment
# Comments aren't run
# They provide human-readable description
# Python comments start with #
print("This is run")  # This is not
```

## 📦 Variables

Variable names can contain letters, numbers, and the underscore (`_`).

```python
a = 1
b = 2
print(a)      # 1
print(a + b)  # 3

language = "Python"
print("I love " + language)  # I love Python
```

Values stored in variables can be changed.

```python
favorite_subject = "math"
print(favorite_subject)      # math
favorite_subject = "science"
print(favorite_subject)      # science
```

## ❓ Conditionals

`if` statements test a condition and run some code if that condition is `True`. If the condition is `False`, those code won't be run.

```python
if 5 > 2:
    print("5 > 2 evaluates to True.")
    print("So the code under the if statement is run.")
    print("Notice how we are indented by a few spaces.")

if 1 == 3:  # Testing for equality
    print("I won't run.")
    print("1 is not equal to 3.")
```

`else` means **otherwise**, and follows `if` statements. If the `if` condition is `False`, the `else` will run.

```python
if 5 < 2:
    print("Is 5 less than 2?")
    print("No! So I won't be run.")
else:
    print("I will be run instead!")
```

`elif` combines `else` and `if`. These are only tested if the `if`s and `elif`s above them were all `False`.

```python
if False:
    print("Not run.")
elif True:
    print("Will run.")
else:
    print("Won't run.")
```

Typical conditionals:

```python
if condition_a:
    # Some code (run if condition_a is True)
elif condition_b:
    # Some code (run if condition_a is False AND condition_b is True)
else:
    # Some code (run if condition_a is False AND condition_b is False)
```

## 🔄 `while` loops

`while` loops run some code **while** some condition is `True`.

```python
i = 0
while i < 4:
    print(i)
    i += 1  # Increment i by 1 (add 1 to i)
# Will print 0, 1, 2, 3
```

Syntax:

```python
while CONDITION:
    SOME_CODE
```

`SOME_CODE` will be run `while` `CONDITION` is `True`.

## 🎲 Random numbers

To generate random integers in Python, we use the `random` module's `randint` function.

Firstly, import the `random` module.

```python
import random
```

Now we can use `random.randint(a, b)` to get a random number between `a` and `b` (including `a` and `b`).

```python
print(random.randint(1, 3))  # Can be 1, 2, or 3
```

## 🤖 Functions

Functions are blocks of code that run when called.

```python
def function_name(inputs):
    do_some_things
    return some_data  # Optional
```

Example:

```python
def f(x):
    return x ** 2  # x squared

print(f(2))  # 4
print(f(9))  # 81
```

## 📃 Lists

The `list` data type stores collections of data.

```python
my_tasks = ["stay alive", "do homework", "drink water", "eat"]
```
