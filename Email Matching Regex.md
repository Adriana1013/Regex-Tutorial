# Regex tutorial - Matching an Email 

In this tutorial you'll learn about regex which is short for regualr expressions. It's a series of special characters that allow you to search certain pattern criteria. Below you'll find all of the components of a regex broken down for you when it comes to matching an email. 

## Summary
As mentioned regular expressions or regex creates a pattern or series of characters that allows you to search specific criteria. This regex will allow you to match any email address within your search: 
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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
As you can see the anchors that are used in the email matching regex are the ^ and $. In the beginning of the expression we use the ^ to indicate the beginning of the string and the $ indicates the end of it.

### Quantifiers
The quantifiers are the meta characters that tell you the quantity or how many characters to match after the anchors. For email matching we see that the + sign is used to indicate 1 or more characters in the first half of the expression. Then we see the + sign used again in the second half along with {} brackets to indicate the minium and maxium between 2-6 characters. 

You can see the breakdown here: 
/^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

### Grouping Constructs
The expression is grouped by username, domain and extension. This is the grouping for the username with letters between a through z and 0 through 9 characters[a-z0-9_\.-], this is for the domain that [\da-z\.-] and here is for the extension of .com with parameters of letters a thorugh z and a min of 2 and max of 6 characters [a-z\.]{2,6}

### Bracket Expressions
The bracket expressions here [] tell you the character specific parameters that need to be validated. In our email matching case we see that the username needs allows letters and numbers.

### Character Classes
The character class here is the \d that tells you it will match any digit between 0 and 9. 

### The OR Operator
The OR operator | gives the option to match either of the acceptable parameters. 

### Flags
Flags give your regex additional criteria by which it will define the search. For example you can use "i" to flag the search is case sensitive, "g" can flag a search for all matches, "m" will flag multiline code. There are more flags that can be used as well.

### Character Escapes
Character escapes allow you to escape characters that are most common 
## Author
This tutorial was written by Adriana Villegas, a current marketer taking a coding bootcamp. [Github](https://github.com/Adriana1013)
