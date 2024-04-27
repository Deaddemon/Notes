# How Java Works

Java applications are platform-independent, meaning they can run on any machine.

## JVM (Java Virtual Machine)

The Java Virtual Machine is platform-dependent and only understands bytecode. Even with multiple files, we need to specify the first file containing the `main` method, which has a particular signature: `public static void main(String[] args)`. The bytecode files have an extension of `.class`.

## JRE (Java Runtime Environment)

The Java Runtime Environment consists of the JVM along with some libraries. It's essential for executing Java applications.

## JDK (Java Development Kit)

Developers use the Java Development Kit, which is not necessary for running Java applications on different machines. It includes the JRE, which in turn includes the JVM and libraries.

# Variables

Java is a strongly-typed language, meaning variables must be declared with their types.

## Data Types

- `long l = 5679L;`
- `byte by = 127;`
- `short sh = 558;`
- `boolean b = true;`
- `float f = 5.8f;`
- `char c = 'd';`

## Type Casting

Type casting allows for explicit conversion between data types.
