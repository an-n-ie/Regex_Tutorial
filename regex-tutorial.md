# Regex Tutorial: Matching a Hex Value

A tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does.

## Summary

To put it simply, regex is an input validator when a specific format is required from the user. We will be breaking down the components of a regex used to match a hex value. Hex values are a special code that represents colors using the hexadecimal color code format.

The following is an example: `/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

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
`/^`#?([a-f0-9]{6}|[a-f0-9]{3})`$/`

Anchors are used at the beginning and end of an expression. `^` and `$` are your anchors. Any character after the `^` indicates the start of a string while anything before the `$` indicates the end.

### Quantifiers
/^#`?`([a-f0-9]`{6}`|[a-f0-9]`{3}`)$/

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. Quantifier characters are `?`, `*`, `+`,  and `{}`. `?` matches zero or one time. `*` matches zero or more times. `+` matches one or more times. `{}` is dependent on the integer inside. So for this case `{6}` matches 6 times and `{3}` matches 3. `{6,}` matches at least 6 times. `{3,6}`matches from 3 to 6 times.

### Grouping Constructs
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### Bracket Expressions
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### Character Classes
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### The OR Operator
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### Flags
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

### Character Escapes
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

# Author
/^#?([a-f0-9]{6}|[a-f0-9]{3})$/

Annie Hoang is an OSU Coding Bootcamp student.

GitHub: https://github.com/an-n-ie 

## Sources
https://medium.com/factory-mind

https://en.wikipedia.org/wiki/Regular_expression 

https://learn.microsoft.com/en-us/dotnet/standard/base-types/quantifiers-in-regular-expressions


