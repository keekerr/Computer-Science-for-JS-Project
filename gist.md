# Computer Science for JavaScript Challenge: Regex Tutorial

## Subject
* Matching an Email – /^([a-z0-9_\.-]+)@([\da-z\.-]+)\.([a-z\.]{2,6})$/

## Summary

In order to better under stand the Regex expression listed above, it is important to understand each of its components.

"^" - This component of the Regex expression indicates that the email address must start at the begining of the expression.

"([a-z0-9_\.-]+)" - This componenet of the Regex expression is the part of the expression that is matching the username of the email addresses. (e.g. the keeley.s.sprouse in keeley.s.sprouse@gmail.com).

"@" - This component of the Regex expression looks for the @ symbol that is located between the username section of an email and the domain name the email belongs to. (e.g. the @ in keeley.s.sprouse@gmail.com).

"([\da-z\.-]+)" - This component of the Regex expression is the part that matches the domain the email belongs to. (e.g. the gmail in keeley.s.sprouse@gmail.com).

"\." -  This component of the Regex expression is the part that matches the character located between the email addess domain and the top level domain (e.g. the . in keeley.s.sprouse@gmail.com).

"([a-z\.]{2,6})" - This component of the Regex expression is the part that matched the top domain of the email (e.g. the com in keeley.s.sprouse@gmail.com

"$" - This component of the Regex expression indicates that the email address must be complete at the end of the expression.

With these definitions in mind, we are able to see that this Regex expression is used to validate email addresses. 
It takes in an email address, checks to make sure that it matches the set format for an email address (i.e. username, a character that separates the username from the domain name, the domain name, the character that separates the domain name from the top level domain name and then the domain name),
and then determines if the input email address is valid or not.

This expression can also be used to set whoch characters can be used in an email address.

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Grouping Constructs](#grouping-constructs)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)
- [Flags](#flags)
- [Character Escapes](#character-escapes)
- [About the Author](#about-the-author)
- [Important Links](#important-links)
- [References](#references)

## Regex Components

### Anchors

Anchors, in relation to a Regex expression, are the special characters that set the boundaries or position in a string. 
An example of this can be seen in the expression above with the use of the carrot (^) and dollar sign ($). 

Some other examples of commonly used anchors can be seen in the characters "\b" (match spaces between strings) and "\A" (very similar to the character "^" but with a few more use restrictions".

### Quantifiers

Quantifiers, in relation to a Regex expression, include characters like Asteriks (*), Plus signs (+), Question marks (?) and Curly Braces ({}).
Quantifiers help to set characters that should be matched in the given string. 

An example of this can be seen in the expression above in the character "{}" (Specifices an exact number of occurances  for the preceding characters i.e. the charaters that are matched in this part of the expression can be any in the lower case range given (a-z) and should be composed of 2-6 characters.

### Grouping Constructs

Grouping Constructs, in relation to a Regex expression, allow for multiple characters to be expressed as a single group/entity.
The character used to indicate a grouping construct are parenthesis ().
Grouping Constructs can be used to capture information that must be referencesd at a later date.

### Bracket Expressions

Bracket Expressions, in relation to a Regex expression, help to match a specific character to a set of characters. 
The character used to indicate a Bracket Expression are a set of brackets [].

### Character Classes

Character Claases, in regard to Regex expressions, help to define a set of characters that can make up a valid input.

### The OR Operator

OR Operators, in regard to Regex expressions, allows for several patterns to be considered a match. 
The character than is used to indicate an OR Operator is the vertical bar symbol |.

### Flags

Flags, in regard to Regex expressions, help to create paramters for the execution of the expression.
Single letter character are used to indicate a a Flag.

### Character Escapes

Character Escpaes, in regard to Regex expressions, are a collection of characters that are given a specific definition. 

## About the Author

Keeley Kerr

* Github: https://github.com/keekerr
* Porfolio: https://keekerr.github.io/Initial-Portfolio/
* LinkedIn: https://www.linkedin.com/in/keeleykerr/
* Email: keeley.s.sprouse@gmailcom

## Important Links

* Github Repo:
* Gist: 

## References

* https://javascript.plainenglish.io/regular-expressions-brackets-f2d6f69ffe13
* https://learn.microsoft.com/en-us/dotnet/standard/base-types/regular-expression-language-quick-reference
* https://www.codeguage.com/courses/regexp/flags
