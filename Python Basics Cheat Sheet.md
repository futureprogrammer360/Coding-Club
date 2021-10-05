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
