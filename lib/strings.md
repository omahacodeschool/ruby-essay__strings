---
title: Strings
instructor_notes: Feel free to re-organize the headings (or add/remove headings) below. We included the headings for your benefit, but it's 100% fine if you want to write your responses in some different structure.
---

# What is a String?

A string object can basically be viewed as a container that holds a sequence of one or more bytes of data. Most of the time, these bytes generally respresent characters that reference written human language. There are, of course, exceptions in more advanced situations. 
the value of strings are generally enclosed in single or double quotation marks 'like this' "or this." Double quotations allow for escape sequences--single quotations does not.
For Ruby, the default chatacter set is ASCII. However, it is possible to use other encoding sets, such as UTF-8 or $KCODE.

# What are some examples of information that would be Strings as opposed to some other data type?

Strings required when attempting to facilitate user interactions or input. If the program needs to ask the user a question, it must do so via a string. 
Any sort of user response is captured in a string.Even if the user enters a number via a response, it generally needs to convert the string into an integer.

# What is one way, using Ruby, to retrieve the 6th character in a String like `"Ada Lovelace"`? How about the 8th character? What happens if you try to retrieve the value of the _99th_ character (Or any character that doesn't exist)?

to retrieve the 6th character, you could use: "Ada Lovelace"[5] # => 'O' 
To retrieve the 8th character, you could use: "Ada Lovelace"[7] # => 'E'
If you attempted to find the 99th character in the aformentioned string, it would simply return nil, as the string only contains 12 bytes total. 

# The previous question asks about finding, for example, the 6th character in a String. Is it possible to find the **-6th** (Notice the negative symbol!) character in a String? What does that even mean?

Yes, it is possible. It would be C . when using a negative number, Ruby will count backwards, right to left from the length of the string, starting at -1.

# What is one way, using Ruby, to replace certain characters in a string with some other set of characters? For example, given `"Sumeet Jain"`, how would you replace all of the `e` characters in my name with exclamation marks? (So it would be `"Sum!!t Jain"`.)
"Sumeet Jain".gsub!(/e/, "!")

