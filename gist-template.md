# Regex Tutorial: Matching a Hex Value

This file is intended to explain the details of how a specific regular expression works. This particular regular expression is used to match a HEX value. The description below will detail each component of the regular expression and how it works. 

## Summary

Today we will be evaluating the following regular expressions used to match HEX values:

`/^#?([a-f0-9]{6}|[a-f0-9]{3})$/`

Description below will provide details  of the anchors, quantifiers, OR operator, character classes, grouping and capturing and bracket expressions used in this regular expression.


## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)

## Regex Components

### Anchors

Anchor: ^ 
Code Snipet: `/^#`

Description: 
Anchors are a different breed. They do not match any character at all. Rather they assert something about the string (e.g. beginning, end)
The caret `^` marks the begining of the string, by repeating the frist character or word you will mark the end of the srting

Example: `^This` indicates that the string must begin with `This`

The # symbol indicates that the number has been written in hex format. This system uses two hex digits for each colour, eg #FF6600.

Anchor: $
Code Snipet: `$/`

Description: 
Matches the end of the string. Similar to the ^ anchor, $ is used to check if a string fully matches a pattern. However, $ asserts the pattern to the end of the string, not the beginning.

Example: `end$` indicates that the string must end with `end`.

In our case end of string must match with the 3 or 6 character pattern identified before the $ anchor. The 3 or 6 character pattern is described in more detail under Quantifiers.

### Quantifiers

Quantifier: ?
Code Snipet: `/^#?`

Description: ? implies a boolean value, 0 or 1. Typically, this makes the preceding symbol/character optional.

Example: This could be used to distinguish between British and American spelling in a string e.g. colour vs color -- the regex would colou?r

In our regex, the quantifier ? indicates that the character # preceding the quantifier ? is optional. It's optional for # to appear at the beginning of the expression.

### OR Operator

### Character Classes

### Grouping Constructs

### Bracket Expressions

### Greedy and Lazy Match

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
