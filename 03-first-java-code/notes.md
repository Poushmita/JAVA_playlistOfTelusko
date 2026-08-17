# Video 03 — Writing Your First Java Code

**Source:** Telusko Core Java lesson by Navin Reddy  
**Notes prepared by:** Poushmita Paul  

> These are independent study notes based on the lesson. They are not official Telusko notes.

## What this lesson covers

- VS Code workspace basics
- Creating a Java source file
- Using the integrated terminal
- Checking `java` and `javac`
- `.java` files
- JShell for quick experiments
- Console output
- The basic compile → run workflow

## VS Code basics

Useful areas of the VS Code workspace include:

| Area | Purpose |
|---|---|
| Explorer | View folders and source files |
| Search | Find text/files |
| Extensions | Add language support and tools |
| Run & Debug | Run and debug programs |
| Terminal | Execute commands inside VS Code |

## Create a workspace

For the first program, create a folder and open it in VS Code. Source files can be created inside that folder.

## Verify Java from the terminal

```bash
java --version
javac --version
```

The lesson emphasizes that Java is used to run a program while `javac` is the compiler used to compile Java source code.

## Java source files

Java source files use the `.java` extension.

```text
Hello.java
```

Examples of other extensions discussed:

- C → `.c`
- C++ → `.cpp`
- JavaScript → `.js`
- Java → `.java`

## JShell

**JShell** is an interactive Java environment useful for quick experiments.

Example:

```text
jshell
2 + 3
9 - 6
```

You can also print text:

```java
System.out.println("Hello World");
```

JShell is useful for experimentation, while regular Java source files are used to build structured programs/applications.

## Printing output

The lesson introduces:

```java
System.out.println("Hello World");
```

Remember for now:

- Text goes inside double quotes.
- A semicolon terminates the statement.
- `println()` prints output and moves to a new line.

## Basic compile → run workflow

```text
Write .java source
      ↓
Compile with javac
      ↓
Run the program with Java
```

Example compilation command:

```bash
javac Hello.java
```

The lesson ends by showing that a Java source file needs additional structure before this simple statement can run as a complete application.

## JShell vs Java source files

| Aspect | JShell | Java source file |
|---|---|---|
| Best for | Quick experiments | Programs/applications |
| Workflow | Interactive | Write → compile → run |
| Structure | Minimal | Structured Java code |

## Common beginner mistakes

- Forgetting `.java` in the file name.
- Confusing `java` and `javac`.
- Forgetting `;`.
- Forgetting double quotes around text.
- Running compilation commands from the wrong directory.
- Expecting a complete Java source file to behave exactly like JShell.

## Quick revision questions

- What does `.java` mean?
- What is `javac`?
- What is JShell used for?
- Why are double quotes needed around text?
- What is the basic Java write → compile → run workflow?

## One-minute summary

This lesson moves from installation into actual Java programming. You learn how to create a Java source file, use VS Code's terminal, experiment with JShell, print output, and understand the initial compile → run workflow. The next step is learning the structure required inside a Java application.
