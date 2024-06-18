# Regex
Regular expressions (regex) are powerful tools used in programming for searching, matching, and manipulating text. They allow 
developers to define complex search patterns, making them invaluable for tasks like data validation, parsing, and transformation.

## Summary
In this tutorial, we will explore thr regex pattern /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. This pattern is commonly used 
for validating email addresses. I will explain each part of the regexm including anchors, quantifiers, and character classes, to help get a better
understanding on how it defines the search pattern for a valid email address.


## Table of Contents
- [Anchors](#Anchors)
- [Quantifiers](#Quantifiers)
- [OR Operator](#OROperator)
- [Character Classes](#CharacterClasses)
- [Flags](#Flags)
- [Grouping and Capturing](#GroupingandCapturing)
- [Bracket Expressions](#BrackeExpressions)
- [Greedy and Lazy Match](#GreedyandLazyMatch)
- [Boundaries](#Boundaries)
- [Back-references](#Back-references)
- [Look-ahead and Look-behind](#Look-aheadandLook-behind)


## Regex Components

### Anchors
Anchors are used to specify the position within the text. In this regex /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/, '^' denotes the start of 
the string anf the '$' denotes the end of the string.

### Quantifiers
Quantifiers define the number of occurances of a charactor or group. In this regex, '{2,6}' specifies that the preceding character class must 
occur between 2 and 6 times.

### OR Operator
The OR operator (`|`) is used to match one pattern or another. While not explicitly used in our regex, it's important to understand its purpose. 

### Character Classes
Character classes are used to define a set of charactors. In our regex, `[a-z0-9_\.-]` matches any lowercase letter, digit, underscore, dot, or hyphen.

### Flags
Flags are optional parameters that modify the behavior of the regex. This regex does not use any flags, but common ones include 'i' for case
insensitive matching and 'g' for global matching.

### Grouping and Capturing
Grouping and capturing are used to create sub patterns. In this regex, `([a-z0-9_\.-]+)` captures the local part of the email address,
`([\da-z\.-]+)` captures the domain name, and `([a-z\.]{2,6})` captures the top-level domain.

### Bracket Expressions
Bracket expressions are used to match any one of the enclosed charactors. In this regex, `[a-z0-9_\.-]` is a bracket expression.

### Greedy and Lazy Match
Greedy matches try to match as much text as possible. while lazy matches try to match as little as possible. THis regex uses greedy matching by default.

### Boundaries
Boundaries are used to match positions between charactors. This regex does not explicitly use boundary matchers like `/b` or `/B`.

### Back-references
Back-references allow you to reuse part of the regex match in the pattern. This regex does not use back-refernces.

### Look-ahead and Look-behind
Look-ahead and look-behind assertions are used to match a group before or after a specific pattern. This regex does not use these assertions.

## Author
Written by Nicole Ables. You can find more of my work on my GitHub https://github.com/nicoleables.
