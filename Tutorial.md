# Title (replace with your title)

Developer.js Regex Tutorial

## Summary

<!-- Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary. -->

REGEX, or Regular Expression, is a sequence of characters that specifies a search pattern, 
like  ` /[0-9a-z]/gi `, which will look for every instance of numbers 0-9, and letters a-z, ignoring case sensitivity.

These patters can be used to manipualte strings in many ways such as finding characters, replacing characters, validating user input, and more. 

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
Anchors are a type of character that specify something about the string or how the search pattern should be implemented 
<br />For example:
<br />` $ ` matches a charcater at the end of a line, while
<br />` ^ ` matches a character at the beginning of a line

### Quantifiers
Quantifiers in regular expressions specify how many times a character, group of characters, or type of characters need to appear for there to be a match  
<br />For example:
<br />` * ` allows you to match a string that is followed by zero or more of the character immediately before the ` * `
<br />` + ` allows you to match a string that is followed by one or more of the character immediately before the ` + `
<br />` ? ` allows you to match a string that is followed by zero or one of the character immediately before the ` ? `
<br />` {} ` allows you to match a string that is followed by the range of characters defined inside the ` {} `


### Grouping Constructs
Grouping Constructs symbolize a subexpression inside a regular expression. Done by using *paranthesis* `  ( ) `, Grouping Constructs allow more specific manipulations of a string by breaking it down into substrings. 
<br />For example:
<br />` 1(23) ` Creates a group to match with ` (23) `
<br />` 1(?:23)* ` Disables this group from matching
<br />` 1(?<Dummy>23) ` Names this group *Dummy*

### Bracket Expressions
Bracket expressions allow characters to be grouped together inside brackets so that any character inside will return a match
<br />For example:
<br />` [xyx] ` will return a match if the string contains either an ` x `, ` y `, or ` z `


### Character Classes
Character classes define characters or sets of characters in which a regular expression must or must not contain a match.
<br />For example:
<br /> ` \d ` matches a numary character
<br /> ` \w ` matches a alphabetic character
<br /> ` \s ` matches a whitespace
<br />` . ` matches any character

### The OR Operator
The Or Operator ` |  or []` is a logical operator you can put into you regex that will allow you to match with a string that contains a character defined by the operator. 
<br />For example:
<br />` a (b|c) `
<br />` a [bc] `
<br />This means that your regex will return a match if there is an ` a ` followed by either ` b ` or ` c `

### Flags
Flags are specials letters you can place at the end of your regex to denote a special way to handle the search.
<br />For example:
<br />Placing `  i ` at the end of the regex will ignore case-sensitivity ` /jkL/i ` will match ` JKl `
<br />Placing `  g ` at the end of the regex will not return after the first match is found
<br />Placing ` m ` at the end of the regex will allow ` ^ ` and ` $ ` to match at the end of a line, instead of a whole string

### Character Escapes
Character escapes are special functions that are started with a ` \ `, and allow the regex to be specified, as well as allowing you to search for characters that are reserved in regex like ` $ ^ * () [] {} ` and so on.
<br />For example:
<br />` \b ` will only return a match at a word boundary 
<br />` \t ` will only return a match at a tab boundary 
<br />` \x020 ` will only return a match at a space boundary
<br />` \$ ` will allow a match to a ` $ ` character to return

In addition to these, there are several other Character Escapes that are useful in regex. You can find a link to a table of these on *Microsoft's* site here: https://docs.microsoft.com/en-us/dotnet/standard/base-types/character-escapes-in-regular-expressions


## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
