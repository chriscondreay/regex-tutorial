# Matching URL Regex

This is a tutorial of how to use the phone number regex and why we would use it in some of our code. In this gist template we will go through the tutorial and what the different expression elements mean and what they are representing through the table of contents.

## Summary

The phone number regex is a regular expression that allows people to put in a phone number and the regex converts that phone number or list of number with dashes so that the user doesn't have to put them in manually and the regex allows the server/webpage/javascript to read as a phone number ex:###-###-####

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
The anchor tags are are characters ^ and $ that both represent a string like in js strings. Putting the anchors ^ and $ is almost the same as " ". In the phone number regex `/^[\+]?[(]?[0-9]{3}[)]?[-\s\.]?[0-9]{3}[-\s\.]?[0-9]{4,6}$/` The anchors can be seen here before and at the end of the regex signifying the beginning and the end of the characters.
### Quantifiers
Quatifiers set the limits of the string that the regex matches, or individual section of the string. In this regex, the quantifiers are those surrounded in curly brackets `{}` which are `{3}` indicating that whatever number the user inputs, it should only be 3 characters long.
### Grouping Constructs
Grouping constructs are sections that are broken up using parenthesis(). By using these, we are grouping sections of the regex and use what is known as a subexpression. Normally grouping constructs can be demonstrated as so `(abc):(xyz)`. The first part of this subexpression is looking for a string that matches "abc" precisely as is the with the second. However, the two are separated by a colon, so rightfully "abc:xyz" would work, but "bca:yzx" would not.
### Bracket Expressions
Bracket Expressions is anything that's insdie a set of square brackets (`[]`) hense the name given. In this regex I gave, the contents that are in the bracket expressions is anything that has to do with the numbers, for example every character and number 0-9 has brackets around it to represent that any number indicated is valid. This would output (555)-555-5555, but not (abc)-abc-abcd as they are numeric and not numbers.
### Character Classes

### The OR Operator
Typically in a regex, whern we have characters in brackets like `[a-z0-9_-]` it is searching fo rthe alphanumeric characters OR two special characters "_" and "-". The OR operator is usually constructed in a regex when dealing with a grouping construct or between two different grouping constructs. The OR operator 
### Flags

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
