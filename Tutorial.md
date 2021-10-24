# Title (replace with your title)

Developer.js Regex Tutorial

## Summary

<!-- Briefly summarize the regex you will be describing and what you will explain. Include a code snippet of the regex. Replace this text with your summary. -->

REGEX, or Regular Expression, is a sequence of characters that specifies a search pattern, 
like  ``` /[0-9a-z]/gi ```, which will look for every instance of numbers 0-9, and letters a-z, ignoring case sensitivity.

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
For example:
``` $ ``` matches a charcater at the end of a line, while
``` ^ ``` matches a character at the beginning of a line

### Quantifiers
Quantifiers in regular expressions specify how many times a character, group of characters, or type of characters need to appear for there to be a match  
For example:
``` * ``` allows you to match a string that is followed by zero or more of the character immediately before the ``` * ```
``` + ``` allows you to match a string that is followed by one or more of the character immediately before the ``` + ```
``` ? ``` allows you to match a string that is followed by zero or one of the character immediately before the ``` ? ```
``` {} ``` allows you to match a string that is followed by the range of characters defined inside the ``` {} ```


### Grouping Constructs
Grouping Constructs symbolize a subexpression inside a regular expression. Done by using *paranthesis* ```  ( ) ```, Grouping Constructs allow more specific manipulations of a string by breaking it down into substrings. 
For example:
``` 1(23) ``` Creates a group to match with ``` (23) ```
``` 1(?:23)* ``` Disables this group from matching
``` 1(?<Dummy>23) ``` Names this group *Dummy*

### Bracket Expressions
Bracket expressions allow characters to be grouped together inside brackets so that any character inside will return a match
For example:
``` [xyx] ``` will return a match if the string contains either an ``` x ```, ``` y ```, or ``` z ```


### Character Classes
Character classes define characters or sets of characters in which a regular expression must or must not contain a match.
For example:
``` \d ``` matches a numary character
``` \w ``` matches a alphabetic character
``` \s ``` matches a whitespace
``` . ``` matches any character

### The OR Operator
The Or Operator ``` |  or []``` is a logical operator you can put into you regex that will allow you to match with a string that contains a character defined by the operator. 
For example:
``` a (b|c) ```
``` a [bc] ```
This means that your regex will return a match if there is an ``` a ``` followed by either ``` b ``` or ``` c ```

### Flags
Flags are specials letters you can place at the end of your regex to denote a special way to handle the search.
For example:
Placing ```  i ``` at the end of the regex will ignore case-sensitivity ``` /jkL/i ``` will match ``` JKl ```
Placing ```  g ``` at the end of the regex will not return after the first match is found
Placing ``` m ``` at the end of the regex will allow ``` ^ ``` and ``` $ ``` to match at the end of a line, instead of a whole string

### Character Escapes

## Author

A short section about the author with a link to the author's GitHub profile (replace with your information and a link to your profile)
