# Email Regex Tutorial

In this tutorial we will be going over an expression using multiple different strings. These are put together to create a valid email address.  

## Summary
In this tutorial we will be looking at the expression today. /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

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

### Anchors
A regular anchor expression starts with ^ and will end with $.
### Quantifiers
In the example above I used {2, 6} as a quantifier. This is used to secify how long the input can be. It can be between 2-6 characrtors long.
### OR Operator
The OR operator is the '|' symble. It is used to seperate two components of an expression. It could be this or it could be this.
### Character Classes
Character classes are things within our expression that tell use what type if informaton to expect. In the expression ubove we have [a-z] this means you can select and letter from a-z. Same with nubers [0-9] means you can use any number 0-9. 
### Flags
Flags are modifiers for you expression. 

i: Ignore Casing, upper or lower case has no differance.

g: Global, this lets you search for all matches not just one.

s: dot all, allows a . to match new character.

m: multiline, multiline mode matches not only at the beginning and the end of the string, but also at start and end of line.

y: sticky, searching the position of a text.

u: unicode, has full unicode abilities. 

These can be used after the // in an expression.
### Grouping and Capturing
Our example has 3 groups. These groups are used to put information together. 1. peter @ 2. Gmail 3. .com (peter@gmail.com)
### Bracket Expressions
In our example we have 3 sets of bracket, they look like this []. These brackets open and close the different sets of information.

#1: [a-z0-9_\.-] This set has a-z characters, numbers 0-9 or underscores, periods and hyphens.

#2: [\da-z\.-] Has all digits case sensitive characters from a-z with periods and hyphens.

#3:[a-z\.] a-z case sensitive with a period.
### Greedy and Lazy Match
In our example we used greedy quantifiers these are + and {}, this allows the expression to be as long as it has to be. Lazy quantifiers would appear +? or {}? these will make the system make the quickest match.
### Boundaries
Boundaries are used to isolate parts of an expression by using \b. You could use man\b this would grab the word man in the word mankind.
## Author
Created my Peter McClelland. Github is https://github.com/PeterwMcClelland
