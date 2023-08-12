# Regex-Tutorial

- Computer Science for JavaScript Challenge

## Summary

RegEx stands for: regular expression; it's a string of text allowing you to create patterns that will help match, locate, and manage text.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)

## Regex Components

### Anchors

- `^` : indicates the beginning of a string
- `$` : indicate the ending of a string

Anchors expression's are ^ to start and $ to end.
### Quantifiers

- `+` : connects the users email + email service + .com
- `{2,6}` : allows a match range of 2-6 characters, for characters a-z

This expression has is a + to communicate there is another sequence to be matched as a greedy quantifier. 
Additionally {2,6} as another greedy quantifier to specify the input should be a minimun of 2 charactors and a max of 6.

### Grouping Constructs

Grouping is done with the round brackets or parentheses and allows to to group a certain part of the regular expression together.

- `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

This expression would be split like so:

- `([a-z0-9\.-]+)` : matches the users email name
- `([\da-z\.-]+)` : matches the email service
- `([a-z\.-]{2,6})` : captures the .com

### Bracket Expressions

- `[a-z0-9_\.-]` : matching characters a-z, 0-9, "_","-", and "." (case sensitive)
- `[\da-z_\.-]` : matching a digit 0-9 and characters a-z, "-", and "." (case sensitive)
- `[a-z_\.]` : matching any character a-z and "." (case sensitive)

### Character Classes

- `\d` : matches a single character 0-9. 

### The OR Operator

- `"OR"` syntax is denoted with a vertical line character "|"

- If you are looking for programming languages: HTML, CSS, javascript the corresponding RegEx would look like: `html|css|javascript(script)`
### Flags

Flags are optional parameters that we can add to a plain expression to make it search in a different way. Each flag is denoted by a sinlge alphabetic character, and servesdifferent purposes in modifying the expression's searching behaviour.

- `i` (Ignore Casing) Makes the expression search case-insensitively.
- `g` (Global) Makes the expression search for all occurences.
- `s` (Dot All) Makes the wild character . match newlines as well.
- `m` (Multiline) Makes the boundary characters ^ and $ match the beginning and ending of every single line instead of the beginning and ending of the whole string.
- `y` (Sticky) Makes the expression start its searching from the index indicated in its lastIndex property.
- `u` (Unicode) Makes the expression assume individual characters as code points, not code units, and thus match 32-bit characters as well.

### Character Escapes

As previously mentioned, we use the `\` backslash to "escape" the following character.

- For characters that are usually treated literally, the `\` indicates that the next character is special and NOT to be interpreted literally.
- For characters that are usually treated specially, the `\` indicates that the next character is not special and SHOULD be interpreted literally. As in `(https?:\/\/)`

## Author

Find me on GitHub: Prototype-1309
