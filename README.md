# Regex-Tutorial for matching an email

Regular Expressions are convenient and useful ways to search for a certain letter or phrase in your string.

## Summary

This is a tutorial for showing how to verify an email using a string called Regular Expression or Regex. You can using this as a way to search for and verify emails are legitimate.

Matching an Email= /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)

## Regex Components

A Regex must start and end with "/" and is composed of a string which can contain:
    - any lowercase letters between a-z
    - any numbers between 0-9
    - an underscore or hyphen
    - between 3-16 characters long

Here are two examples:
    -Matching a Username= /^[a-z0-9_-]{3,16}$/
    -Matching an Email= /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

### Anchors

Anchors contain a "^" and "$" in them and bother have their own specific use.

The "^" anchor is used when a string begins with a character that follows it while the "$" is used in the string when a character ends.

### Quantifiers

Quantifiers are used to find the set or range of characters we are looking for adn the {} indicates in this example that email string can be between 2 and 6 characters long.

### OR Operator

Characters within the [] will return a match as long as it's a letter from a-z, number from 0-9, dash or dot for the first part of the email example listed above while the second pair of square brackets is any digit, letters from a-z, dot or dash.

### Character Classes

\d- Matches any digit and is equivalent to the bracket expression [0-9].

\w—Matches any alphanumeric character from the basic Latin alphabet, including the underscore (_) and is equivalent to the bracket expression [A-Za-z0-9_].

\s- Matches a single whitespace character, including tabs and line breaks.

### Flags

A regex must be wrapped in slash \\ characters and are placed at the beggining and end of a Regex. Flags are placed at the end, after the second slash and define additional limits for the regex. You can use the six optional flags separately or together in any order.

### Grouping and Capturing

() or parenthesis are used for grouping parts of the expression and the email example can be broken down into 3 parts of groups.Each grouping definies a part of the email address.

-Part ONE: ([a-z0-9_.-]+) defines the part before the @ in your email
-Part TWO: ([\da-z.-]+) definies the part after the @ but before the "."
-Part THREE: ([a-z.]{2,6}) defines the part after the "." 

EX: Example@example.com
      P1     P2      P3

### Bracket Expressions

Bracket Expressions are when you use the square brackets "[]" and the represent a set of characters you want to match and target characters we want to include.

## Author

JuanCarlos Roa Jr. Full Stack Developer
