# Email Regex Tutorial 

I am going to give a step by step tutorial on how this regex functions.  

## Summary

Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary.

/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/     

This is a regular expression that is used to validate an email address.

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
^ - The caret symbol indicates the start of the string.<br/>
([a-z0-9_\.-]+) - This is a capturing group that matches the username part of the email address. It matches one or more lowercase letters, numbers, underscores, dots, and hyphens.<br/>
@ - This matches the "@" symbol that separates the username and domain name parts of the email address.<br/>
([\da-z\.-]+) - This is another capturing group that matches the domain name part of the email address. It matches one or more alphanumeric characters, dots, and hyphens.<br/>
\\. - This matches the dot between the domain name and the top-level domain.<br/>
([a-z\.]{2,6}) - This is the final capturing group that matches the top-level domain of the email address. It matches lowercase letters and dots, and there must be between 2 to 6 of these characters.<br/>
$ - The dollar sign indicates the end of the string.<br/>



### Anchors

^ - This anchor matches the start of the string, indicating that the email address should start with the pattern defined in the regular expression. <br/>
$ - This anchor matches the end of the string, indicating that the email address should end with the pattern defined in the regular expression.<br/>

### Quantifiers
\+ - This quantifier means "one or more". It is used in both the first and second capturing groups to match one or more characters of the defined character set. Specifically, it matches one or more lowercase letters, digits, underscores, dots, or hyphens in the first capturing group, and one or more digits, lowercase letters, dots, or hyphens in the second capturing group.

{2,6} - This is a quantifier that matches between 2 and 6 characters of the preceding character set. It is used in the third capturing group to match between 2 and 6 lowercase letters or dots.
### OR Operator
[a-z0-9_.-] - This is a character class that matches any one character that is a lowercase letter, a digit, an underscore, a dot, or a hyphen.

[a-z.] - This is another character class that matches any one character that is a lowercase letter or a dot.
### Character Classes
[a-z0-9_.-] - This character class matches any one character that is a lowercase letter, digit, underscore, dot, or hyphen. It is used in the first capturing group to match the characters in the username part of the email address.

[\da-z.-] - This character class matches any one character that is a digit, lowercase letter, dot, or hyphen. It is used in the second capturing group to match the characters in the domain name part of the email address.

[a-z.] - This character class matches any one character that is a lowercase letter or a dot. It is used in the third capturing group to match the characters in the top-level domain part of the email address.
### Flags
In the regular expression /^([a-z0-9_.-]+)@([\da-z.-]+).([a-z.]{2,6})$/, there are no flags being used. Flags are optional parameters that can be added to the end of a regular expression to modify how the regular expression is matched.
<br/>Some common flags include "i" to indicate a case-insensitive match and "g" to indicate a global match that finds all occurrences of a pattern in a string.
### Grouping and Capturing

### Bracket Expressions
[a-z0-9_.-] - This is a bracket expression that matches any one character that is a lowercase letter, digit, underscore, dot, or hyphen. It is used in the first capturing group to match the characters in the username part of the email address.

[a-z.] - This is another bracket expression that matches any one character that is a lowercase letter or a dot. It is used in the third capturing group to match the characters in the top-level domain part of the email address.
### Greedy and Lazy Match
There is no example of greedy or lazy matching in this expression.  Greedy and lazy quantifiers can be used to control the behavior of regular expressions when matching substrings. Greedy quantifiers will match as much as possible, while lazy quantifiers will match as little as possible.
### Boundaries
The boundaries in this regular expression are represented by the caret (^) and dollar sign ($). These are known as the start-of-string and end-of-string anchors, respectively.

The ^ anchor specifies that the pattern should match at the beginning of the string, while the $ anchor specifies that it should match at the end of the string. Together, they ensure that the entire string matches the pattern, and not just a substring within the string.
### Back-references
There are no back references in this regex.
### Look-ahead and Look-behind
There are no look-ahead or look-behind in this regular expression. 
## Author
https://github.com/isaacp5454
I am a brand new web developer trying to understand the ways of life. 





