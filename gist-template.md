***Your Challenge this week is to create a tutorial that explains how a specific regular expression, or regex, functions by breaking down each part of the expression and describing what it does. ****

# Regex

Regex, also known as regular expressions, are patterns used to match character combinations in strings.  It is useful in extracting information from any text.

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

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
Search pattern for regex has boundaries by 2 slash characters /.
For example: /abc/

### Anchors
Anchors are asserted at a particular place in the search.
^ : beginning of string
$ : end of string
For example:  ^The will match any string that starts with The.

### Quantifiers
Specifies how many characters a string must present in the input for a match. Quantifiers are * + ? and {}.
For example: abc* will match a string that has ab followed by zero or more 'c'.

### OR Operator
OR operators are | or [].
For example: a(b|c) matches a string that has 'a' followed by 'b' or 'c'.

### Character Classes
Character classes distinguishes different kinds of characters such as letters and numbers. 
*[] - one character:
    - Ex: [abc] means 'a' or 'b' or 'c'
*[^abc] - any character except a, b, or c
*\d - one numerical character from [0-9]
*\w - one character from [a-zA-Z0-9_]
*\s - matches white space characters.


### Flags
A flag value is added at the end of the slash character 
g : global, which does not return after the first match.  It restarts the after the end of the last search.
m : multi-line, enable with ^ and $. This will match the start and end of a line.
i : insensitive, which makes the whole expression case-insensitive

### Grouping and Capturing
(), this operator is used to extract information from strings or data. Groups will be shown in an array. 

### Bracket Expressions
[], means exactly one character.
For example, [abc] means a or b or c.


### Greedy and Lazy Match
Quantifiers, * + {}, are greedy operators.  They will match as much as possible.
For example, 
"This is a <div>simple div</div> test."
<.+> will show a match of <div>simple div</div>

To make a Lazy match, you can add a ?  operator.  Using the above example, a search with <.+?> will return just the div tag, <div> and </div>

### Boundaries
\b, is an anchor, like the caret ^. It matches positions where one side is a word character and the other side is not a word character.
\B,  matches all positions where \b doesn't match.

### Back-references
\1, matches the same text that was matched by the first capturing group.
\2, matches the same text that was matched by the second capturing group.
The same goes for \3, \4 and etc.

### Look-ahead and Look-behind
(?=),
Example: d(?=r), matches a d only if is followed by r, but r will not be part of the overall match

(?<=),
Example: (?<=r)d, matches a d only if it comes before r, but r will not be part of the overall match.

## Author

Thuy Nguyen, is a software engineer student.  She's studying at the University of Central Florida.  GitHub link: https://github.com/ThuyTTTN
