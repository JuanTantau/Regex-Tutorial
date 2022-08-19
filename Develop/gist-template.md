# Regex match a hexadecimal

A regular expression is a sequence of characters that specifies a search pattern in text. Usually such patterns are used by string-searching algorithms for "find" or "find and replace" operations on strings, or for input validation.

## Summary
Today I will be explaining this Regex (regular expression) /^#?([a-f0-9]{6}|[a-f0-9]{3})$/

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [OR Operator](#or-operator)
- [Character Classes](#character-classes)
- [Flags](#flags)
- [Grouping and Capturing](#grouping-and-capturing)
- [Bracket Expressions](#bracket-expressions)
- [Greedy and Lazy Match](#greedy-and-lazy-match)
- [Boundaries](#boundaries)
- [Back-references](#back-references)
- [Look-ahead and Look-behind](#look-ahead-and-look-behind)

## Regex Components

### Anchors
 The anchors in our example are "^" and "$" also known as "position meta characters". They are placed in the beginning/end. Why? because the "^" marks the beginning of the stringg and the "$" mark the closing of the string.
### Quantifiers
In our example we have two types of quantifiers, we have "?" and "{n}". "?" matches any preceding character 0 or 1 times. the quantifier "{n}" was used twice in our example "{6}" and "{3}". These characters match exactly the preceding character n-times.
### OR Operator
our regex has one big group, divided by an OR operator |. In the group ([a-f0-9]{6}|[a-f0-9]{3}) we have two expresions: [a-f0-9]{6} and [a-f0-9]{3}. That just means that our example will match any of those two expresions.
### Character Classes
In our example our "character classes" are repeated twice "[a-f0-9]". A character class matches any character enclosed in brackets.
### Grouping and Capturing
This regex expresion has one big group "([a-f0-9]{6}|[a-f0-9]{3})". This grouping is used in combination with an OR operator.
## Author
Juan L. Tantau

Github: https://github.com/JuanTantau

