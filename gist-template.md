# Regex Basics Tutorial

Short for regular expression, it's a sequence of characters that defines search patterns. It uses a variety of characters such as "@^[a".
Regex's purpose is to be used for Javascript to enable and validate URL's, emails, and usernames.

## Summary

For this tutorial, Regex has a unique set of string language for emails; which is "/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/". Its function's purpose is for a user to input a valid email address that consists with a number of characters preceding the @ symbol, followed by a domain such as yahoo for instance.

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


## Anchors

Anchors share a different purpose from characters. While the symhols themselves are special characters, they're actually served for positions before and after characters. For instance, "^" the caret anchor copies the previous text of code. The "$" matches the after text. To validate an email address, you must put it in between the anchors.

**^\S{1,}@\S{2,}\.\S{2,}$**





## Quantifiers

Quantifiers set limits for a string that your regex matches (or an individual section of the string). They frequently include the minimum and maximum number of characters that your regex is looking for.

In this instance, if you want to set a limit for an email address, you'd have to do this.

**^\S{1,}@\S{2,}\.\S{2,}{3,16}$**


## Grouping Constructs

Grouping constructs delineate the subexpressions of a regular expression and capture the substrings of an input string.

To do this with an email, you'd have to input this:

/^((abc):(xyz)0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Bracket Expressions

Anything inside a set of square brackets ([]) represents a range of characters that we want to match are called **bracket expressions**.

For an email, you'd have to do this:

**^[a-z]\S{1,}@\S{2,}\.\S{2,}$**

## Character Classes

Character classes define sets of characters inside a string to match any input.

An example would be "\d", which matches any numeral digit.


## The OR Operator

The **OR Operator** uses this syntax "|" to group and differentiate constructs.

An example would be:

**(a|b|c):(x|y|z)**

## Flags

Flags are placed at the end of a regex, after the second slash, and they define additional functionality or limits for the regex.

/.../

This is used for every aspect of string.


## Character Escapes

The backslash in a regular expression precedes a literal character. If you put a backslash after a curly bracket for instance, it'll look for the curly bracket.

## Author

* Regex Tutorial made by Mohamed Farah

* Github Username: MoeFar95

* https://github.com/MoeFar95
