# Regex - Matching an email
You may ask what is a Regular expression? (Regex for short)
They are a series of special characters that define a search pattern.
## Summary
In this tutorial I will show you how to match a Email.
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
^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$

As you can see here this entire set of numbers and special characters are wrapped in (/). 
Regex is a literal so they need to wrapped in this slash character (/).

### Anchors
You may be wondering what is a anchor?  A anchor matches a position before, after, or between characters.

Example

^ - This anchor signifies a string that begins with the characters that follow it. (Keep in mind that that Regex is case sensitive so ^at and ^At are different)
$ - This anchor signifies a string that ends with the characters that precede it.

So in our example we have ^([a-z0-9_\.-]+) this is stating that we need characters that are lower case a-z.


### Flags
In regex we have these things called flags they come at the end after the (/).

Example of some flags:
//g - Global search this will show all the possible matches in a string.
//i - Case insensitive should be ignored when attempting a match in a string

### Quantifiers



### OR Operator

### Character Classes

### Grouping and Capturing

### Bracket Expressions

In our example we see ([]) a lot lets talk about why we see these brackets. These are called bracket expressions they represent a range of characters we want to match, they are also known as positive character group,
because they outline the characters we want to include.

So for example:
[a-z] - The string will only contain letters through a-z but, remember regex is case sensitive so to include upper case we would need to do [a-zA-Z].

[0-9] - The string can contain any number between 0-9

[_-] - The string can contain underscore or hyphen. The underscore and hyphen are called special characters. So are any non-alphanumeric character.

The following examples will work using regex:
'isaac'

'isaac2'

'is-aac'

'23456'

'_-_-'

If we were to use the string 'Isaac' well that would not work so we would need to figure what we can do. The way we can get this to work is to use the (^) this is called the negative character group.
You would place the (^) to the beginning of the expression inside the brackets.

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

Isaac Yanez 