# Title (replace with your title)

This tutorial is meant for you to gain a better understanding and apretiation for regex and also for those that do not know what it is to learn what it is. Regex or regular expressons are a sequence of characters that form a serch pattern for things such as letters, numbers or any other characters within a string. regex is a great way for you to validate data that has been inputed such as a phone number, address, name and anything else. below is one exapmle of data that can be validated.

## Summary

The regex that I will be useing as an exampil wil be a passsword validation that you can use to as it sounds validate a password ^(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.*[a-zA-Z]).{8,}$  

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
Regex is made up of components and each has a diffrent function/meaning and below i will go through each one useing the password validator as an exaple 

### Anchors
Anchors are unique in that they will match positions with a string not character such as the beginning, end word boundary, and not word boundary. We will go though the anchors below.

In our exampile ^(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.*[a-zA-Z]).{8,}$ The beginning is marked by a ^ the end is marked by the $ and other anchors to note are the word boundery is \b and not word boundery \B

### Quantifiers
Quantifiers will indicate that the preceding token has to be mached a certain number of times. They are by default, quantifiers are greedy, and will match as many characters as possible. We will go though the quantifiers below.

In our exampile ^(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.*[a-zA-Z]).{8,}$

The {8,} will match 3 or more

### OR Operator
There is whats called a or operator it is represanted by a | symbol however it is not in our exaple.

### Character Classes
A character class will match a character from a specific set. there are a number of predefined character classes and you can also define your own sets with them

In our exampile ^(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.*[a-zA-Z]).{8,}$

The . would mean any character except newline. the \d matches any digit character (0-9) also equivalent to [0-9]

### Flags
The expression flags change how the exprssion is interpreted.
Flags follow the closing forward slash of the expression.
Examples would be.

i-Ignore case. this will make the expression case sensitive.

g-Global search this will store the index of the last match.

m-Multi line will case the beginning and end anchore to match the start and end of a line insted of the whole string.

u-Unicode this will allow extended unicode escapes in the form \x{FFFF}.

y-Sticky this will match from its last index position and ignores the global search flag.

s-Dotall this will cuse dot to match any charcter

### Grouping and Capturing
Grouping will allow you to combine a sequence of tokens to operate on them together. Capture groups can be referenced by a backreference and accessed separately in the results.

In our exampile ^(?=.*\d)(?=.*[a-z])(?=.*[A-Z])(?=.*[a-zA-Z]).{8,}$

(ABC) Groups multiple tokens together and creates a capture group for extracting a substring or using a backreference.

(?<name>ABC) Creates a capturing group that can be referenced via the specified name.

\1 Matches the results of a capture group. For example \1 matches the results of the first capture group & \3 matches the third.

(?:ABC) Groups multiple tokens together without creating a capture group.

### Bracket Expressions
Bracket expressions match a specific set of single charcter. It will match a specific set of multi-character collating elements, based on the non empty set of list expressions contained in the bracket [] expression 

### Greedy and Lazy Match
The greedy and lazy match makes the preceding quantifier lazy, causing it to match as few characters as possible. By default, quantifiers are greedy, and will match as many characters as possible. and is a ? symbol

### Boundaries
Boundaries are a position between \w and \W to define a word character

### Back-references
The back references are commands that refer to previous sections of the expression they are specified with a \ and a single digit \1

### Look-ahead and Look-behind
Lookahead/lookbehind lets you match a group before (lookbehind) or after (lookahead) your main pattern without including it in the result.

## Author

This was writen by Cameron Charlesworth 
GitHub: 
