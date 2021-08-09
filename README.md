
## Regex Tutorial 

## Summary

Today I will be explaining the different components of a Regular Expression, which
what is commonly known as regex and they are a group of special charactors which make
up a search pattern. The one that I picked was one that matches any email address from 
the domains yahoo.com, gmail.com and hotmail.com. 

                               `(\W|^)[\w.\-]{0,25}@(yahoo|hotmail|gmail)\.com(\W|$)`

## Table of Contents

- [Anchors](#anchors)
- [Quantifiers](#quantifiers)
- [Bracket Expressions](#bracket-expressions)
- [Character Classes](#character-classes)
- [The OR Operator](#the-or-operator)

## Regex Components

### Anchors

These can be expressed in two different ways, like this ^ and like this $. The ^ signifies a string
the begins with the charactors that follow it and the $ signifies the end. Pulled from "match any email address", 
below you can see that the ^ is used. With the incorporating the \W with the ^ simply means that this string
can start with anything number 0-9, any letter a-z, A-Z and even the _. My regex example uses both of them as 
you can see below. 

                                       `(\W|^)`    `(\W|$)`

### Quantifiers

These are what set limits for the string that you are trying to match up to the regex you plug in. 
They usually are using the min and max number of charactors that your particular regex is searching for.
For example in the email regex that i am picking apart below, you can see below an example of the min,max
written out. 

                                           ` {0,25} `

### Bracket Expressions

So this pretty unique as anything inside the square brackets [] will be representing a scope of charactors 
that it wants to match. They are also called Positive Charactor Group and that is why simply it is highlighting 
the actual charactors it wants to include. In my regex example snippet below basically it is saying that all the 
charactors in the basic latin alphabet it can use and that is what it wants to highlight by putting it in the []. 

                                           ` [\w.\-] `

### Character Classes

These define a group of charactors which any of them can be found in a input string for it to render a match. 
A good example from my regex example is the ` \w ` which means any alphanumeric character from the basic Latin
alphabet incluing the underscore is acceptable in the hunt for these! 

### The OR Operator

This is also called the Alternation Operator is expressed usually in brackets, which we talked about above in the 
bracket expressions section, and it is written like (| or \| ) and it is self explanatory that it means this or that. In
my regex example below it is written that it will except entries from any of these options; yahoo, hotmail or gmail.

                                       `(yahoo|hotmail|gmail)`

## Author

My name is kaivon tolooee and I am just graduating from a 
Full Stack Coding Bootcamp . Please be gentle! :) 
https://github.com/kaivont85