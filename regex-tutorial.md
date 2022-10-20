# Regex Tutorial: Matching a Hex Value

A tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does.

## Summary

A regular expression is a sequence of characters that defines a specific pattern. Regex can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They can also be used to validate input required from the user. We will be breaking down the components of a regex used to match a hex value. Hex values are special codes that represent colors using the hexadecimal color code format.

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

Quantifiers specify how many instances of a character, group, or character class must be present in the input for a match to be found. Quantifier characters are `?`, which matches zero or one time; `*`, which matches zero or more times; `+` matches one or more times;  and `{}` is dependent on the integer inside. So for this example, `{6}` matches 6 times and `{3}` matches 3. Other examples include `{6,}`, which matches at least 6 times and `{3,6}`, which matches from 3 to 6.

### Grouping Constructs
/^#?`([a-f0-9]{6}|[a-f0-9]{3})`$/

Grouping outlines the subexpression(s) of a regular expression. It also captures the substring(s) of an input string.

### Bracket Expressions
/^#?(`[a-f0-9]`{6}|`[a-f0-9]`{3})$/

Similiar to grouping except `[]` outlines a character class or quantifier statement.

### Character Classes
/^#?(`[a-f0-9]`{6}|`[a-f0-9]`{3})$/

Character classes allow matches to only certain types characters. In this example, `a-f` allows letters a-f and `0-9` allows digits 0-9.

### The OR Operator
/^#?([a-f0-9]{6}`|`[a-f0-9]{3})$/

The OR operator is indicated by the `|`. In this example, it is similar to saying that either `[a-f0-9]{6}` or `[a-f0-9]{3}` is valid since hex values can be 6 or 3 characters with letters a-f and digits 0-9.

# Author

Annie Hoang is an OSU Coding Bootcamp student.

GitHub: https://github.com/an-n-ie 

## Sources
https://medium.com/factory-mind

https://en.wikipedia.org/wiki/Regular_expression 

https://learn.microsoft.com/en-us/dotnet/standard/base-types/regular-expressions

https://www.regular-expressions.info/



