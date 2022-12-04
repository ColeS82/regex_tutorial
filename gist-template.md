# Regular Expressions (regex)

Regular expressions are a very useful tool for developer becuase is a equivalant to the search function in a word processor yet regular expressions can search specific patterns in code.  The power in the regex is that can search patterns and or ranges.  For example, one can search for words containing b or c in specific patterns.  This tutorial will cover the expression, /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/.

## Summary

Reular Expressions are sets of strings that search for specic patterns in code.  They are a valuable tool for developers in many different languages as most languages will use the same expressions.

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
A regular expression is a syntax for a search pattern/criteria.  There are many components that can make up a regular expression such as anchors, quantifies, bracket expressions, character classes, the OR Operator, Flags, Character Escapes and author.

### Anchors
Anchors are special characters like a ^.  The carrot in this case is an anchor that siginals the beginning or end of a string and the patter begins after the ^.  Another anchors is the $.  The $ signals the end of a search pattern. 

### Quantifiers
Quatnifiers limit the amount of charaters to be searched.  ({6, 10}) sets a limit to match a string of 6 to 10 characters to be searched.  A ? can be used at the end to reduce the matches as much as possible

### Grouping Constructs
As the name implies, grouping constructs are used to group parts of the expression into sections.  Grouping is accomplised by the use of ()

### Bracket Expressions
Bracket expressions create a list of characters to be searched for inside ([]) and creates range of characters to be searched for.  Any character in the list will be searched for.  In our example these set the searches for 

### Character Classes
A “character class” tells the regex engine to match only one out of several characters. If placed between [] to match word that may have variations. For example, use gr[ae]y to match either gray or grey. Very useful if you do not know whether the document you are searching through is written in American or British English.

### The OR Operator
The OR operator searches for a list of terms as a whole and by individual characteristics with |.  An example is (and|or|then).  In this example the OR operator will find those specific words independently.

### Flags
Flags are added at the end of regex to add additional features and there are six of them. The three most common are g, i, and m. The g flag runs a global search to find all possible matches. The i flag means that case should be ignored in the search. The m flag means an input should be treated as multiple lines. Using the example code the user can add a g at the end and make the regex look like this: /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. This will search for the matching pattern globally.

### Character Escapes
Character escapes allow the user to use a term literally instead of the meaning in regex. In order to use a character escape you have to put a slash (\) in front of the character. This will make the character lose its meaning in the regex. For instance, instead of using ^ to represent the start of a regex, the user can put a slash in front and have the program search for a ^ in the program. In the example code /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/. all of the .'s will be literal.

## Author
This report was created by Cole Sexson.  Cole sexson is a studen in full stack web development.  You can contact Cole at https://github.com/ColeS82

