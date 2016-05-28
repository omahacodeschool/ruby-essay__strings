---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string is a line of text or values typically created by using quotations.

# What are some examples of information that would be Strings as opposed to some other data type?

Strings are created by enclosing values with quotations and by doing such any 
mathematical operator used on a string will return a string value instead of an 
integer value like some other data types would. If someone wants to only convey the 
meaning of the number two they will need to put 2 in quotations. Otherwise while 
2 by itself still is indeed the number two, the language the computer reads it as
is a fixnum, not a string.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

Given a string of a specific length, using a code (like string_name[integer])to call for a character within
the string should be performed by defining the string as a variable ex. a_string = "string"
and then performing the ruby command to retrieve the nth value of a_string. Given 
that a string has n length, where the first character is the zero-ith position, 
a request for the n+1 position will return a nil response.

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

A request for a character with a positive number will start at the beginning of 
the string and count its way til the end of the string. Using a negative number 
will start the count at the end of the string and work its way from right to left.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)

The gsub command in the rubymonk link is used by first defining the a set of characters
(e in the questions example) that the user wants to replace followed by the value 
that is to replace that set of characters (! from the example) within the string.
The sub command is used to just replace the first defined character with the 
replacement value. G in gsub can be interpreted as global.
