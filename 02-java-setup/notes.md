# Video 02 — Setting Up Java: JDK, VS Code & PATH

**Source:** Telusko Core Java lesson by Navin Reddy  
**Notes prepared by:** Poushmita Paul  

> These are independent study notes based on the lesson. They are not official Telusko notes.

## What this lesson covers

- Editors vs IDEs
- Why the course uses VS Code
- JDK installation
- Java versions and LTS
- Choosing a JDK for the operating system
- PATH/environment-variable configuration on Windows
- Verifying `java` and `javac`

## Editor vs IDE

A basic editor lets you type code. An **IDE (Integrated Development Environment)** can provide a broader development workflow, including editing, compilation, running, debugging, and project tooling.

Examples mentioned in the lesson include VS Code, Eclipse, IntelliJ IDEA, and NetBeans.

## Why VS Code?

The lesson uses **Visual Studio Code** because it is lightweight and flexible while still providing development features through extensions.

## JDK — Java Development Kit

The **JDK (Java Development Kit)** is the development kit used to create and compile Java programs.

The lesson demonstrates installing an Oracle JDK and discusses open-source Java implementations as alternatives.

## Java versions and LTS

Java receives regular releases. Not every release is an LTS release.

**LTS = Long-Term Support**.

The lesson uses **Java 17** because it is an LTS release in the context of the original recording.

> **Version note:** The Java-version discussion here reflects the lesson's recording context. For current projects, check the currently supported JDK release and project requirements.

## Operating-system choice

The JDK download depends on the operating system and, for some platforms, the hardware architecture.

Examples mentioned:

- Windows
- Linux
- macOS with Apple silicon or Intel

The underlying Java language concepts remain the same across operating systems.

## PATH configuration on Windows

If Java is installed but the command prompt cannot find `javac`, the PATH environment variable may not contain the JDK's `bin` directory.

Typical idea:

```text
JDK installation
   ↓
JDK\bin
   ↓
Add this directory to PATH
```

After changing PATH, restart the command prompt/terminal and verify again.

## Verify the installation

Check the Java runtime:

```bash
java --version
```

Check the compiler:

```bash
javac --version
```

If both commands return a version, Java and the compiler are available in the terminal.

## Key takeaways

- JDK is needed for Java development.
- An IDE/editor improves the development experience.
- LTS means Long-Term Support.
- On Windows, PATH may need to include the JDK `bin` directory.
- Verify installation with `java --version` and `javac --version`.

## Common beginner problems

- Installing a JDK but not updating PATH.
- Opening an old terminal after changing PATH.
- Installing the wrong OS/architecture package.
- Confusing the JDK with an editor such as VS Code.

## Quick revision questions

- What does IDE stand for?
- What is the difference between an editor and an IDE?
- What does JDK stand for?
- What does LTS mean?
- Why might `javac` fail even after Java installation?
- Which two commands verify Java and the compiler?

## One-minute summary

Before writing Java programs, you need a development environment. The lesson uses VS Code plus a JDK. The JDK provides the Java development tools, while VS Code provides the editing environment. On Windows, the JDK's `bin` directory may need to be added to PATH so terminal commands such as `java` and `javac` work from any location.
