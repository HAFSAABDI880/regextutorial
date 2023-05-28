Read me 
Regular Expressions (RegExp)

'regex', is a method used in various languages including JavaScript which find patterns in a text. It's used mostly to validate a user input and to search through a body of text.
There are two main ways of created a Regex object; either by using literal syntax, the second way is by using the RegExp() constructor.

The literal syntax (/pattern/) uses forward slashes to wrap the regular expression pattern and does not use quotation marks, whereas the constructor syntax ("pattern") uses quotation marks and is not enclosed between slashes.

One of the way Regex could be used is to validate user input.

I'll be using this line of code throughout my tutorial:
/^(https?:\/\/)?([\da-z\.-]+)\.([a-z\.]{2,6})([\/\w \.-]*)*\/?$/

Table of Contents
Anchors
Quantifiers
Grouping Constructs
Bracket Expressions
Character Classes
The OR Operator
Flags
Character Escapes

Regex Components
Anchors
An anchor in regex represents the position of the string from the beginning to its .end. The caret ^ is positioned before the first character in the string. For example in our line of code:

/^(https?://)?([\da-z.-]+).([a-z.]{2,6})([/\w .-])/?$/

The caret is found after the forward slash used in the literal syntax, this indicates that the string starts from the opening parenthesis and not at the beginning line of code.

Similarly, the dollar sign $ shows the ending of the string and is to be found at the end of the code line.

Quantifiers
Quantifiers shows how many instances a character is present in the line of code. Quantifiers can be applied to the individual characters and classes contained by the parentheses.

Grouping Constructs
Regex uses parenthesis to group substrings of an input string to combine a sequence of literals and pattern characters.

There are a few different types of grouping constructors:

x|y -> Matches either "x" or "y".
/(foo)/ -> Capturing group. Matches and remembers the match character.
(?:x) -> Non-capturing group. Does not remember the match.
[xyz] -> Character class. Matches any one of the characters in the range.
a-c] -> You can specify the range of characters by using a hyphen. But if the hyphen is at the beginning or ending of the square brackets then it is taken as a literal hyphen.

Bracket Expressions
Bracket Expressions are characters enclosed by a square bracket matching any character within the brackets.
Character Classes
There are two types of character classes: character escapes, and character classes. A character escape uses a backslash to make the characters located in a square bracket invalid. It’s used as a literal interpretation. In this example, an escape can be seen as a backslash. A character class is any of the characters that are found in the regex sequence.

The OR Operator
The or expression give the operator to use either one function or the other. The common regular expression for this operators is the(|).

Referencesrrrr
https://coding-boot-camp.github.io/full-stack/computer-science/regex-tutorial