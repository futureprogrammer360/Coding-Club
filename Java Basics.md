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
