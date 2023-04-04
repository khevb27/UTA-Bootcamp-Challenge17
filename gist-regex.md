# Regular Expressions (Regex) Tutorial

Regular expressions, or regex for short, are a powerful tool for working with text data. They allow you to search for and manipulate text based on patterns of characters. In this tutorial, we will cover the basics of regular expressions, including the syntax and metacharacters commonly used in regexes. By the end of this tutorial, you should have a basic understanding of how to create and use regular expressions to search for patterns in text data.


## Summary

Here's an example regex that uses several of the components we'll be discusing in this tutorial. This regex matches email addresses that follow a basic format: a string of lowercase letters followed by an @ symbol, another string of lowercase letters, a dot, and then 2 or 3 lowercase letters.

    /^[a-z]+@[a-z]+\.[a-z]{2,3}$/i


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
Anchors are used to match a specific position within a string, rather than a character or set of characters. The two most common anchors are:
 
    ^ - which matches the beginning of a string
 
    $ - which matches the end of a string
 
 For example, the regex ^hello would match any string that starts with "hello", while the regex world$ would match any string that ends with "world".

### Quantifiers
Quantifiers specify how many times a character or group should be matched. 

    The * quantifier matches zero or more occurrences
    
    The + quantifier matches one or more occurrences
     
Other quantifiers include:

    ? - for zero or one occurrence

    {m,n} - for between m and n occurrences

### Grouping Constructs
Grouping constructs are used to group together multiple characters or groups so that they can be treated as a single unit. This can be useful for applying a quantifier or other metacharacter to the entire group. 
    The most common grouping construct is (), which creates a capturing group

### Bracket Expressions
Bracket expressions, or character sets, are used to match any one character from a specified set. 

    For example, the bracket expression [aeiou] would match any vowel.

### Character Classes
Character classes are similar to bracket expressions, but instead of specifying a set of characters, they match a specific type of character. 
Common character classes include:

    \d - for digits
    \s - for whitespace
    \w - for word characters (letters, digits, and underscores)

### The OR Operator
The OR operator | allows you to match one of several possible patterns. 
    For example, the regex cat|dog would match either "cat" or "dog".

### Flags
Flags are optional modifiers that can be added to the end of a regex to change the way the regex is interpreted or executed. 
Common flags include:

    i - for case-insensitive matching
    g - for global matching
    m - for multi-lane matching

### Character Escapes
Character escapes are used to match characters that have special meaning in regex. 
For example:

    The . character is normally used to match any character, but if you want to match a literal . character, you can use the escape sequence \.

    Other common escape sequences include \n for a newline character and \t for a tab character

## Author

Khevin Brahmbhatt
- https://github.com/khevb27