# Regex-Tutorial

17. Computer Science for JavaScript Challenge

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

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

Anchors expression's are ^ to start and $ to end.
### Quantifiers

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This expression has is a + to communicate there is another sequence to be matched as a greedy quantifier. 
Additionally {2,6} as another greedy quantifier to specify the input should be a minimun of 2 charactors and a max of 6.

### Grouping Constructs

Grouping is done with the round brackets or parentheses and allows to to group a certain part of the regular expression together.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

This expression would be split like so:

1st - ([a-z0-9_\.-]+)

2nd - ([\da-z\.-]+)

3rd - ([a-z\.]{2,6})

### Bracket Expressions

### Character Classes

### The OR Operator

### Flags

Flags are optional parameters that we can add to a plain expression to make it search in a different way. Each flag is denoted by a sinlge alphabetic character, and servesdifferent purposes in modifying the expression's searching behaviour.

i (Ignore Casing) Makes the expression search case-insensitively.
g (Global) Makes the expression search for all occurences.
s (Dot All) Makes the wild character . match newlines as well.
m (Multiline) Makes the boundary characters ^ and $ match the beginning and ending of every single line instead of the beginning and ending of the whole string.
y (Sticky) Makes the expression start its searching from the index indicated in its lastIndex property.
u (Unicode) Makes the expression assume individual characters as code points, not code units, and thus match 32-bit characters as well.

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
