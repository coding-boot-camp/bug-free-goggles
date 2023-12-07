#  Regular Expression (Module 17 Challenge)

Hello All!! The purpose of this gist project is to describe a regular expression and its functionality. Regular expression is a sequence of characters that defines a specific search pattern. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input. This is great for pulling out information from a given body of code as well as being used for validation. For example, this tutorial will follow an example code snippet that can be used to match an email. This tutorial will follow the different components of regular expressions.

## Summary

The tutorial will give specific examples for how the components of regex can be used. The following code can be used to match emails. One use for this code is that it can be used to validate to make sure that an email follows the correct format.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/


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

The anchor is what starts and ends a regular expression. In following example,

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/,

The anchors are the ^ and the $. This code specifically is saying that we are looking for something that starts with

^([a-z0-9_\.-]+)

The anchor means is that if we find a match it has to follow these initial guidelines. It also has to end with

.([a-z\.]{2,6})$.

So, it must start and end with the given parameters within the code. If it does not, then it is not a match.

### Quantifiers

A quantifier is used to determine how many times a specific character or group of characters needs to be present in order to have a match. For instance, if we used the following example in our regex, xyz+ then this will match any string xy followed by at least one z. 

([a-z0-9_\.-]+)

This will match any string that contains a-z, 0-9, _, ., or -. The quantifier + means that it has to contain at least one of this in order to have a match.

### OR Operator

Aside from the given code, OR operators are marked with an |. a popular way this OR operator is used is in date regex, such as:
^(0[1-9]|1[012])[-/.](0[1-9]|[12][0-9]|3[01])[-/.][0-9]{4}$

the first group ^(0[1-9]|1[012]) demonstrates the user can pick a month starting with 0 or"(|)" 1, followed by the sequenced numbers that follow. This operator sets up the regex for controlled alternates.

### Character Classes

Character classes distinguish kinds of characters such as, for example, distinguishing between letters and digits. \d is present in the given matching email code and what it will match a single letter character, a-z, after the @ sign in the email address. Basically ensuring that a letter is matched after the @ in the email and not a number or special character.

### Flags

A flag is an optional parameter to a regex that modifies its behavior of searching. A flag changes the default searching behavior of a regular expression. It makes a regex search in a different way. A flag is denoted using a single lowercase alphabetic character. A regex flag is not used in the matching email code that is being used for this tutorial. A regular expression typically comes in the form:

/regex/

Where the slashes denote where the regular expresssion starts and ends. A flag can be used after the slash to give more guidelines for our matching. The flags are:

g which stands for "global" which will allow for matching all the instances within a string that follow the matching guidelines set in the regular expression.
m which stands for "multiline" which will search line by line rather than searching through a string as a whole.
i which stands for "insensitive" will make the regular expression case-insensitive, so capitals and lower-case letters will not deture the matching.


### Grouping and Capturing

### Bracket Expressions

### Greedy and Lazy Match

### Boundaries

### Back-references

### Look-ahead and Look-behind

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
