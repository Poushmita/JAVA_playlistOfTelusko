# Video 04 — JVM, JRE, JDK, Bytecode & `main()`

**Source:** Telusko Core Java lesson by Navin Reddy  
**Notes prepared by:** Poushmita Paul  

> These are independent study notes based on the lesson. They are not official Telusko notes.

## What this lesson solves

The previous simple Java file did not run as a complete application. This lesson explains the missing structure and the execution model behind Java.

## Java's execution model

The core flow introduced is:

```text
Java source code (.java)
        ↓
   Java compiler (javac)
        ↓
Bytecode (.class)
        ↓
       JVM
        ↓
     Output
```

## Why Java is platform independent

A Java application can run on different machines as long as the required Java runtime environment is available for that platform.

The key idea is:

- The **Java application/bytecode** is designed to be portable.
- The **JVM itself is platform dependent** and is implemented for a specific operating system/platform.

This is the basis of the familiar **Write Once, Run Anywhere (WORA)** idea.

## Bytecode

Java source code is compiled into **bytecode**.

The compiled output uses the `.class` extension.

Example:

```text
Hello.java  →  Hello.class
```

The JVM executes this bytecode rather than the original `.java` source directly.

## `javac`

`javac` is the Java compiler. Its job is to translate Java source code into bytecode.

Example:

```bash
javac Hello.java
```

## The `main()` method

The JVM needs an entry point from which application execution starts. The lesson introduces the standard `main` method signature:

```java
public static void main(String[] args)
```

For now, the important point is to remember the signature. The meaning of each keyword is explained in later lessons.

## Classes

Java is object-oriented, and the lesson introduces the class as the structure required around the program code shown in the example.

The class name in the example is kept the same as the file name.

Basic structure:

```java
public class Hello {
    public static void main(String[] args) {
        System.out.println("Hello World");
    }
}
```

## Compilation creates a `.class` file

After successful compilation, a corresponding `.class` file appears. This file contains the bytecode that the JVM executes.

## Running the program

After compilation, the lesson uses the Java launcher with the **class name**, not the source-file name:

```bash
java Hello
```

The important distinction is:

```text
Compile: javac Hello.java
Run:     java Hello
```

## JDK, JRE and JVM

The lesson presents the following conceptual relationship:

```text
JDK
└── JRE
    └── JVM
```

- **JDK — Java Development Kit:** used by developers and includes development tools.
- **JRE — Java Runtime Environment:** provides the runtime environment needed to run Java applications.
- **JVM — Java Virtual Machine:** executes Java bytecode.

The lesson also describes runtime libraries as part of the JRE.

## Development vs runtime

A developer needs the JDK to create and compile Java applications. A machine that only needs to run an application does not need the full development toolkit in the lesson's model; it needs the runtime components.

## WORA

**Write Once, Run Anywhere** means Java bytecode can be executed on different supported platforms through their compatible Java runtime/JVM.

## Key takeaways

1. Java source code is compiled into bytecode.
2. Bytecode is stored in `.class` files.
3. The JVM executes bytecode.
4. Java applications are portable across supported platforms because each platform provides an appropriate JVM/runtime.
5. The JVM needs a recognized `main()` entry point for a standard application start.
6. The lesson's conceptual hierarchy is JDK → JRE → JVM.

## Quick revision questions

- What is bytecode?
- What does `javac` do?
- Why is Java considered platform independent?
- Why is the JVM platform dependent?
- What is the purpose of `main()`?
- What is the difference between `java Hello` and `javac Hello.java`?
- What do JDK, JRE and JVM stand for?
- What does WORA mean?

## One-minute summary

Java source code is compiled by `javac` into bytecode stored in `.class` files. The JVM executes that bytecode, allowing the same compiled application to run on different supported platforms. A standard Java application has a `main()` entry point inside a class. The lesson also introduces the JDK → JRE → JVM relationship.
