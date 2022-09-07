# 17-Regex Tutorial 

## Summary 

A **regex**, or **regular expression**, is a sequence of characters that defines a specific search pattern. The regex in this tutorial is used to match an HTML tag. When included in code or search algorithms, regular expressions can be used to find certain patterns of characters within a string, or to find and replace a character or sequence of characters within a string. They are also frequently used to validate input. This tutorial will break down the regex's different components as shown in the table of contents.

This tutorial will cover the following regex:

 - Matching an Email: `/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/`

 This regex is particularly useful for validating emails using back-end technologies such as NodeJs and MongoDB. 

## Table of Contents
- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Character Classes](#character-classes)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)


## Regex Components

## Anchors

This regex uses the `^` anchor to denote the beginning of the string and the `$` anchor to signify its ending. In the example above, the content of the email is contained withing the `^` near the beginning and ends with the `$` at the end.

## Quantifiers

This regex makes use of the `+` operator, which is used to connect the user's email name to their email service, and again to the `.com` part of the string. 

Likewise, the quantifier `{2,6}` appears in the regex to indicate that 2 to 6 characters matching matching those within the bracket `[a-z0-9_\.-]` are expected to appear. 

## Character Classes

This regex uses the `\d` character class, which matches a single digit number from 0 to 9. 

## Grouping Constructs

The first grouping in this expression is `([a-z0-9_\.-])`, which matches the user's email name. The second grouping, `([\da-z\.-])` matches the email service's name. The final grouping, `([a-z\.]{2,6})` matches the `.com`.

## Bracket Expressions

The bracket expressions in this regex include the character sets `[a-z0-9_\.-]`, which matches letters from a to z and is case sensitive. It also matches numbers 0 to 9, as well as the following characters, `_`, `-` and `.`. 

## Author

Contact me via [github](https://github.com/jgislaszapata) or [email](mailto:$jesusgibranislas@gmail.com).