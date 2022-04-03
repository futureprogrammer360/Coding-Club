# Java Basics

## 3/28/2022

### Printing things

To print out some text, we use the following code:

```java
System.out.println("The text you want to print");
```

### Data types

Different data types store different types of data.

* `String`s store textual data ("Hello", "Bye")
* `int`s store whole numbers (193, -12381)
* `double`s store decimal numbers (1.31231, -481.23)
* `boolean`s store truth values (`true`, `false`)

### Variables

To make a variable in Java, we specify its data type, its name, and its value.

```java
String greeting = "Hi";
int numberOfWords = 0;
double PI = 3.14;
boolean isRaining = false;
```

### Comments

Sometimes it is helpful to include comments in our code. Comments are ignored by the Java compiler, but humans can read it and better understand the code.

```java
// This is a comment

/*
    This
    is
    a
    multi-line
    comment
*/
```

### User inputs

Getting inputs from the user is not the most straightforward thing in Java.

At the top of your program, you need the line:

```java
import java.util.Scanner;
```

Then, in your `main` method, you need to write this:

```java
Scanner sc = new Scanner(System.in);
```

To finally get inputs from users, here's what you need:

```java
System.out.print("Your name: ");
String name = sc.nextLine();
System.out.println("Hello, " + name);
```

### Mad Libs

Now you have all you need to make a mad libs game. Give it a try!

Below is a very short example just for reference.

```java
import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Enter a name: ");
        String name = sc.nextLine();
        System.out.print("Enter a school subject: ");
        String subject = sc.nextLine();
        System.out.print("Enter an adjective: ");
        String adjective = sc.nextLine();

        System.out.println(name + " is a student who thinks that " + subject + " is " + adjective);
    }
}
```

## 4/4/2022

### Conditions

We often want our programs to make decisions. These choices are usually determined by conditions. Conditions are essentially questions we can ask ourselves. For example, *5 > 4* is a condition that checks whether 5 is greater than 4 or not.

```java
System.out.println(5 > 4);
System.out.println(3 == 3);
System.out.println(27 / 9 == 9 / 3);
System.out.println(2.1 != 2.1);

// Comparing String values - use .equals()
System.out.println("Hello".equals("Hello"));
System.out.println("Hello".equals("hi"));
```

### Conditionals

Knowing whether a condition is `true` or `false` does us little good if we don't use that information to do something. Using conditional statements, we can do a certain action **if** a condition is `true` and another action **otherwise** (`else`).

```java
if (5 > 4) {
    System.out.println("5 is greater than 4");
} else {
    System.out.println("5 is not greater than 4 🤔");
}
```

Knowing this in addition to what we learned about user inputs last time, think about how you would write a program simulating a user logging in to their account.

```java
Scanner sc = new Scanner(System.in);

System.out.print("Username: ");
String username = sc.nextLine();

System.out.print("Password: ");
String password = sc.nextLine();

if (username.equals("Some username")) {
    if (password.equals("Some password")) {
        System.out.println("Access granted.");
    } else {
        System.out.println("Incorrect password: are you who you say you are?");
    }
} else {
    System.out.println("Incorrect username: are you who you are?");
}
```

### Adventure Time

With what you have learned so far, you can create a choose-your-own-adventure type of game using conditional statements. Give it a try, and if you need a hint, the program below may be of use.

```java
import java.util.Scanner;

class Main {
    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);

        System.out.print("Do you want to go to school (y/n): ");
        String x = sc.nextLine();
        if (x.equals("y")) {
            System.out.println("You went to school. Why?");
        } else {
            System.out.println("You didn't go to school. Do you want to do homework (y/n): ");
            x = sc.nextLine();
            if (x.equals("y")) {
                System.out.println("You did homework all day long. Why?");
            } else {
                System.out.println("You slept all day.");
            }
        }
    }
}
```
