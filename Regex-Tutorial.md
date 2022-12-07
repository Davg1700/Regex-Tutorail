# Title ( Regex-Tutorail)

Regex-Tutorail

## Summary

This example of regex is used for matching emails.

Matching an Email – /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/

here i will be breaking down the components for what the text above means.

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

The characters ^ and $ are both considered to be anchors.

The ^ anchor signifies a string that begins with the characters that follow it. This could be in one of two formats: 1st is ^The, where the strings "The" or "The person" match, but "the" and "the person" do not. This is because a regex is case-sensitive.

The $ anchor signifies a string that ends with the characters that precede it. Just as with the ^ character, it can be preceded by an exact string or a range of possible matches.

so in our “Matching a email” regex, the string must start and end with something that matches the pattern [a-z0-9_-].

### Quantifiers

taking a look into brackes. the + Matches the pattern one or more times

Quantifiers set the limits of the string that your regex matches (or an individual section of the string

### Grouping Constructs

Grouping Construcsts s fairly straightforward and open-ended about what it accepts.

The primary way you group a section of a regex is by using parentheses (()). Each section within parentheses is known as a subexpression.

### Bracket Expressions

Anything inside a set of square brackets ([]) represents a range of characters that we want to match.

### Character Classes

A character class in a regex defines a set of characters, any one of which can occur in an input string to fulfill a match.

Here are some of the other common character classes:

.—Matches any character except the newline character (\n)

\d—Matches any Arabic numeral digit. This class is equivalent to the bracket expression [0-9].

\w—Matches any alphanumeric character from the basic Latin alphabet, including the underscore (_). This class is equivalent to the bracket expression [A-Za-z0-9_].

\s—Matches a single whitespace character, including tabs and line breaks

### The OR Operator

Remember that a bracket expression does not require the string to meet all of the requirements in the pattern. This means that [a-z0-9_-] searches for alphanumeric characters or the two special characters included in the pattern. Often, you'll want to add this same logic outside of a bracket expression, especially within a grouping construct or between two different grouping constructs.

### Flags

We started this tutorial by explaining that as a literal, a regex must be wrapped in slash characters. The one exception to this rule is with the component known as flags. Flags are placed at the end of a regex, after the second slash, and they define additional functionality or limits for the regex. these are the three you're most likely to encounter:

g—Global search: the regex should be tested against all possible matches in a string.

i—Case-insensitive search: case should be ignored while attempting a match in a string

m—Multi-line search: a multi-line input string should be treated as multiple lines

### Character Escapes

The backslash (\) in a regex escapes a character that otherwise would be interpreted literally. For example, the open curly brace ({) is used to begin a quantifier, but adding a backslash before the open curly brace (\{) means that the regex should look for the open curly brace character instead of beginning to define a quantifier.

## Author

David Delgadillo [here](https://github.com/Davg1700)

## Refrences

link to refrence can be found [here](https://coding-boot-camp.github.io/full-stack/computer-science/regex-tutorial)
