# Video 05 — Variables, Data & the `int` Type

**Source:** Telusko Core Java lesson by Navin Reddy  
**Notes prepared by:** Poushmita Paul  

> These are independent study notes based on the lesson. They are not official Telusko notes.

## What this lesson covers

- Data and processing in applications
- Persistent storage vs temporary storage
- Variables as named storage locations
- Strong typing in Java
- `String` for text
- `int` for integer values
- Assignment operator `=`
- `print()` vs `println()`
- Arithmetic with variables
- Storing intermediate results

## Why applications work with data

Software solves real-world problems by accepting and processing data. A typical application can:

```text
Input → Processing → Storage
```

Data may come from a user, be transformed or calculated, and then be stored for later use.

## Database vs variable

A database provides persistent storage, while a variable is temporary working storage used while the program executes.

| Concept | Purpose |
|---|---|
| Database | Persistent storage |
| Variable | Temporary working storage |

## What is a variable?

A variable can be imagined as a named box that holds a value.

A simplified declaration looks like:

```text
type variableName = value;
```

Example:

```java
int num = 3;
```

Breakdown:

- `int` → type
- `num` → variable name
- `3` → value
- `=` → assignment operator
- `;` → end of statement

## Java is strongly typed

The lesson describes Java as a strongly typed language. When declaring a variable, the programmer specifies the kind of data that variable is intended to hold.

## String — text

Text is represented using `String`.

Example:

```java
String name = "Naveen";
```

## int — integer values

`int` is introduced as a type for integer/whole-number values. The lesson explains that it can represent negative and positive integer values.

Examples:

```java
int num = 5;
int balance = -5;
int score = 10;
```

A decimal such as `6.5` is not an `int`; the lesson defers the appropriate decimal type to a later discussion.

## Assignment operator `=`

The equal sign is the **assignment operator**. It assigns the value/expression on the right to the variable on the left.

```java
int num = 3;
```

Conceptually:

```text
right-hand side → left-hand side
```

## Semicolons and blocks

Normal Java statements end with a semicolon:

```java
int num = 3;
```

Curly-brace blocks are different:

```java
{
    // statements
}
```

## `print()` vs `println()`

| Method | Effect |
|---|---|
| `print()` | Prints and stays on the same line |
| `println()` | Prints and then moves to a new line |

Example:

```java
System.out.println(5);
System.out.println(15);
```

## Arithmetic with variables

Variables can be used in expressions.

```java
int num1 = 3;
int num2 = 5;
System.out.println(num1 + num2);
```

The expression uses the values currently stored in the variables.

## Storing an intermediate result

Instead of printing the expression directly, the result can be stored in another variable:

```java
int num1 = 3;
int num2 = 5;
int result = num1 + num2;
System.out.println(result);
```

This gives the conceptual flow:

```text
Input values → calculation → result variable → output
```

## Compile after changes

After changing the source code, compile again before running the updated program.

```text
Edit/save
   ↓
Compile
   ↓
Run
```

## Common beginner mistakes

- Declaring a variable without a type.
- Trying to store a decimal in an `int` variable.
- Forgetting the semicolon.
- Confusing `=` with comparison.
- Editing code but running an old compiled version because recompilation was skipped.
- Using `print()` when each result is supposed to appear on a separate line.

## Quick revision questions

- What is a variable?
- Why does Java require a variable type?
- What does `int` mean?
- What is `String` used for?
- What does `=` do?
- What is the difference between `print()` and `println()`?
- Can variables be used in arithmetic expressions?
- Why store an intermediate result in another variable?

## One-minute summary

Variables provide named storage for data during program execution. Java is strongly typed, so a variable declaration includes its type. This lesson introduces `String` for text and `int` for integer values, explains assignment with `=`, demonstrates `print()` and `println()`, and shows how variables can be combined in arithmetic and used to store intermediate results.
