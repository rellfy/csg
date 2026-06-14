# General, language-agnostic code style guide

## 1 Document by code explicitness, not comments
Instead of writing comments, refactor the code so that it is explicit.
For example, a comment before a function call should not explain what the function does;
instead, the function name should be descriptive enough so that it is explicit.

Comments should explain how or why something is, not what it is.

**Reason**: readability, less maintancne and invalid comments.

## 2 Small functions
Functions should be very small, with minimal lines.
Complex lines with high cognitive load should be specially isolated into their own functions.

**Reason**: small functions are easy to read, and the function itself serves as documentation.

## 3 Minimal blank lines
If a function is large enough to need many blank lines,
consider creating more functions.

**Reason**: consistency

## 4 Acronyms use PascalCase or camelCase
e.g instead of `ID`, it should be written as either `id` or `Id` depending on the
context (variable vs class name, for example).
The exception is if the name is a static/constant, which uses the UPPER_SNAKE_CASE.

**Reason**: readability.

## 5 Boolean names should be worded as a question
Word boolean names as a question.

For example: `isTrue`, `doesAction`, `shouldDoAction`.

**Reason**: readability, consistency.

## 6 Comments should go above the code
When commenting a line of code, comments should go on the line above it rather than after it.

## 7 Comment capitalisation and punctuation
Comments should start new sentences with a capital letter, and end the sentence with a
full stop.
Sentences can be broken into new lines.

For example, a single line comment:

```
// This is a one line comment.
```

And a multi-line comment:

```
// This is a very in-depth comment
// that goes through a lot of details.
```

**Reason**: consistency

## 8 Comment grammatical person
Comments should be written in the impersonal third person format.

Avoid using "I" or "we" in a comment.

**Reason**: consistency

## 9 Order items in a source code file in order of importance
Source code file items should read in order of importance: high-level, public functions go at the top,
and low-level, private util functions go at the bottom.
The exception for this is that consts, statics and structs go at the top.

