<!--
  Copyright 2020, Gerwin Klein, Régis Décamps, Steve Rowe
  SPDX-License-Identifier: CC-BY-SA-4.0
-->

# Example from the user manual

This is the [example from the user manual](http://jflex.de/manual.html#Example).

This example does not describe the whole lexical structure of Java programs,
but only a small and simplified part of it (some keywords, some operators,
comments and only two kinds of literals). It also shows how to interface with
the LALR parser generator CUP and therefore uses a class `sym` (generated by
CUP), where integer constants for the terminal tokens of the CUP grammar are
declared.

For a full implementation of **Java 1.2**, see [cup-java](../cup-java).

## Build, run, test

### Using Maven

To build and test the lexer:

    mvn test

### Using Ant

To build and test the lexer:

    ant test

### Using Make

To build and test the lexer:

    make test

## Files

* `src/main/jflex/minijava.flex`
  Partial (simplified) specification of Java.
* `src/test/java/jflex/examples/minijava/LexerTest.java`
  Test of the generated lexer.